<template>
    <div class="home">
      <nav class="navbar">
        <h1 class="logo">IE Bank Corp</h1>
        <ul class="nav-links">
          <li><a href="#about">About Us</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
      
      <header class="hero">
        <div class="hero-content">
          <h2>Welcome to IE Bank Corp!</h2>
          <p>Manage your finances with ease and simplicity.</p>
          <button class="primary-button" @click="navigateToAccount">Get Started</button>
        </div>
      </header>
      
      <section id="about" class="about">
        <div class="about-content">
          <h3>Who We Are</h3>
          <p>IE Bank Corp provides smart and friendly banking services designed to meet your needs. We aim to simplify banking for everyone with modern and secure solutions.</p>
        </div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'HomePage',
    methods: {
      navigateToAccount() {
        this.$router.push('/accounts');
      },
    },
  };
  </script>
  
  <style scoped>
  .home {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: #2c3e50;
    margin: 0;
    padding: 0;
    line-height: 1.6;
  }
  
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background-color: #fff;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
  }
  
  .logo {
    font-size: 1.8rem;
    font-weight: bold;
    color: #4CAF50;
  }
  
  .nav-links {
    list-style: none;
    display: flex;
    gap: 1.5rem;
  }
  
  .nav-links a {
    color: #2c3e50;
    text-decoration: none;
    font-size: 1rem;
    transition: color 0.3s;
  }
  
  .nav-links a:hover {
    color: #4CAF50;
  }
  
  .hero {
    background: linear-gradient(135deg, #4CAF50, #81C784);
    padding: 8rem 1rem;
    color: white;
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 60vh;
  }
  
  .hero-content {
    max-width: 600px;
    margin: auto;
  }
  
  .hero h2 {
    font-size: 3rem;
    font-weight: bold;
    margin-bottom: 1rem;
  }
  
  .hero p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
  }
  
  .primary-button {
    background-color: #fff;
    color: #4CAF50;
    border: none;
    padding: 0.75rem 1.5rem;
    font-size: 1rem;
    cursor: pointer;
    border-radius: 30px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
    transition: background-color 0.3s, color 0.3s;
  }
  
  .primary-button:hover {
    background-color: #4CAF50;
    color: #fff;
  }
  
  .about {
    padding: 4rem 2rem;
    background-color: #f9f9f9;
    text-align: center;
  }
  
  .about-content {
    max-width: 800px;
    margin: auto;
  }
  
  .about h3 {
    font-size: 2rem;
    margin-bottom: 1rem;
  }
  
  .about p {
    font-size: 1.1rem;
    color: #555;
  }
  </style>
  