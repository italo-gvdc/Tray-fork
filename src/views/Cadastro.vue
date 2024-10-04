<template>
  <div class="container">
    <header id="header" class="d-flex align-items-center">
      <div class="header-container d-flex align-items-center justify-content-between">
        <div class="logo">
          <h1 class="text-light"><a href="/" class="logo-link"><span>SneakerWorld</span></a></h1>
        </div>
        <nav id="navbar" class="navbar d-flex align-items-center">
          <ul class="d-flex list-unstyled mb-0">
            <li class="nav-item">
              <router-link class="nav-link" to="/">Home</router-link>
            </li>
          </ul>
          <i class="bi bi-list mobile-nav-toggle"></i>
        </nav>
      </div>
    </header>
    

    <div class="registration-container">
      <h2 class="text-center">Cadastro</h2>
      <form @submit.prevent="submitForm" class="registration-form">
        <div class="form-group">
          <label for="nome">Nome:</label>
          <input type="text" id="nome" v-model="formData.nome" class="form-control" required>
        </div>
        <div class="form-group">
          <label for="email">Email:</label>
          <input type="email" id="email" v-model="formData.email" class="form-control" required>
        </div>
        <div class="form-group">
          <label for="senha">Senha:</label>
          <input type="password" id="senha" v-model="formData.senha" class="form-control" required>
        </div>
        <button type="submit" class="btn btn-primary">Cadastrar</button>
        <p v-if="successMessage" class="alert alert-success mt-3">{{ successMessage }}</p>
        <p v-if="errorMessage" class="alert alert-danger mt-3">{{ errorMessage }}</p>
      </form>
    </div>
  </div>
</template>

<script>
import PessoaService from '@/services/PessoaService';

export default {
  name: "CadastroPessoa",
  data() {
    return {
      formData: {
        nome: '',
        email: '',
        senha: ''
      },
      successMessage: '',
      errorMessage: ''
    };
  },
  methods: {
    submitForm() {
      PessoaService.create(this.formData)
        .then(response => {
          this.successMessage = 'Cadastro realizado com sucesso!';
          this.errorMessage = '';
          this.resetForm();
        })
        .catch(error => {
          if (error.response && error.response.status === 500) {
            this.errorMessage = 'Erro no servidor ao realizar o cadastro.';
          } else if (error.response && error.response.status === 400) {
            this.errorMessage = 'Erro ao realizar o cadastro. Verifique seus dados.';
          } else {
            this.errorMessage = 'Erro ao realizar o cadastro. Tente novamente mais tarde.';
          }
          this.successMessage = '';
        });
    },
    resetForm() {
      this.formData.nome = '';
      this.formData.email = '';
      this.formData.senha = '';
    }
  }
};
</script>


<style scoped>
/* Header Styles */
header {
  background-color: #000;
  padding: 15px 20px;
  border-bottom: 1px solid #444;
}

.header-container {
  max-width: 1200px;
  margin: 0 auto;
}

.logo h1 {
  color: white;
  margin: 0;
}

.logo-link {
  text-decoration: none;
  color: white;
}

.navbar .nav-link {
  color: white;
  padding: 10px 20px;
  border-radius: 30px;
  font-weight: 500;
  text-transform: capitalize;
  transition: background-color 0.3s, color 0.3s;
}

.navbar .nav-link:hover {
  background-color: #ff4500;
}

/* Registration Container Styles */
.registration-container {
  max-width: 600px;
  margin: 30px auto;
  padding: 30px;
  background-color: #f9f9f9;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.registration-container h2 {
  font-size: 2rem;
  color: #333;
  margin-bottom: 20px;
}

.registration-form .form-group {
  margin-bottom: 20px;
}

.registration-form label {
  font-weight: 600;
  color: #333;
}

.form-control {
  border-radius: 8px;
  border: 2px solid #ff4500;
  padding: 10px;
  font-size: 1rem;
  color: #333;
}

.form-control:focus {
  border-color: #ff6347;
  box-shadow: 0 0 5px rgba(255, 99, 71, 0.5);
  outline: none;
}

.btn-primary {
  background-color: #ff4500;
  border: none;
  color: white;
  padding: 12px 20px;
  border-radius: 50px;
  font-weight: 600;
  text-transform: uppercase;
  transition: background-color 0.3s;
}

.btn-primary:hover {
  background-color: #ff6347;
}

.alert-success {
  background-color: #d4edda;
  color: #155724;
  padding: 10px;
  border-radius: 8px;
  margin-top: 10px;
}

.alert-danger {
  background-color: #f8d7da;
  color: #721c24;
  padding: 10px;
  border-radius: 8px;
  margin-top: 10px;
}


.container {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  width: 100%;
  margin: 0 auto;
  padding: 20px;
  background-color: #f9f9f9;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

h2 {
  margin-bottom: 20px;
  text-align: center;
  color: #333;
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: block;
  margin-bottom: 5px;
  color: #666;
}

input[type="text"],
input[type="email"],
input[type="password"] {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button[type="submit"] {
  width: 100%;
  padding: 10px;
  background-color: #007bff;
  border: none;
  border-radius: 5px;
  color: #fff;
  cursor: pointer;
}

.alert {
  padding: 10px;
  border-radius: 5px;
  text-align: center;
  margin-top: 10px;
}

.alert-success {
  background-color: #28a745;
  color: #fff;
}

.alert-danger {
  background-color: #dc3545;
  color: #fff;
}
</style>