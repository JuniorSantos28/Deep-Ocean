<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Login - Dark Nature</title>
</head>
<body>
    <section class="login-container">
        <div class="login-box">
            <h2>Login</h2>
            <form>
                <div class="input-group">
                    <input type="email" placeholder="Email" required>
                </div>
                <div class="input-group">
                    <input type="password" placeholder="Senha" required>
                </div>
                <div class="options">
                    <label><input type="checkbox"> Lembre-me</label>
                    <a href="#">Esqueceu a senha?</a>
                </div>
                <button type="submit" class="btn-login">Entrar</button>
                <p class="register-link">Não possui uma conta? <a href="#">Registre-se</a></p>
            </form>
        </div>
    </section>
</body>
</html>

body {
    width: 100%;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    /* Imagem de alta resolução do oceano */
    background: url('https://images.unsplash.com/photo-1518467166778-b88f373ffec7') no-repeat center center/cover;
    background-attachment: fixed;
}

.login-box {
    /* Azul translúcido para combinar com a água */
    background: rgba(10, 45, 70, 0.2); 
    padding: 40px;
    border-radius: 20px;
    backdrop-filter: blur(15px); /* Vidro um pouco mais embaçado */
    -webkit-backdrop-filter: blur(15px);
    border: 1px solid rgba(255, 255, 255, 0.15);
    box-shadow: 0 15px 35px rgba(0, 0, 0, 0.5);
    color: #e0f2f1; /* Branco levemente azulado */
    width: 380px;
}

.btn-login {
    width: 100%;
    padding: 12px;
    border: none;
    border-radius: 8px;
    /* Gradiente que remete à cor da água profunda */
    background: linear-gradient(45deg, #0077be, #00a8cc);
    color: white;
    font-weight: bold;
    cursor: pointer;
    transition: transform 0.3s ease, background 0.3s;
}

.btn-login:hover {
    transform: translateY(-2px);
    background: linear-gradient(45deg, #00a8cc, #0077be);
}

.input-group input::placeholder {
    color: rgba(255, 255, 255, 0.6);
}
