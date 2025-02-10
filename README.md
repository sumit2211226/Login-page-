<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interesting Login Page</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            line-height: 1.5;
        }

        .container {
            display: flex;
            height: 100vh;
        }

        .left-side {
            display: none;
            width: 50%;
            background: linear-gradient(135deg, #a855f7, #ec4899, #ef4444);
            color: white;
            padding: 2rem;
        }

        .right-side {
            width: 100%;
            background-color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 2rem;
        }

        .login-form {
            width: 100%;
            max-width: 400px;
        }

        h1 {
            font-size: 2.25rem;
            font-weight: bold;
            margin-bottom: 1.5rem;
            text-align: center;
        }

        .form-group {
            margin-bottom: 1rem;
        }

        label {
            display: block;
            margin-bottom: 0.5rem;
        }

        input {
            width: 100%;
            padding: 0.5rem;
            border: 1px solid #d1d5db;
            border-radius: 0.375rem;
            font-size: 1rem;
        }

        button {
            width: 100%;
            padding: 0.75rem;
            background-color: #4f46e5;
            color: white;
            border: none;
            border-radius: 0.375rem;
            font-size: 1rem;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #4338ca;
        }

        .signup-link {
            margin-top: 1rem;
            text-align: center;
            font-size: 0.875rem;
            color: #6b7280;
        }

        .signup-link a {
            color: #4f46e5;
            text-decoration: none;
        }

        .signup-link a:hover {
            text-decoration: underline;
        }

        @media (min-width: 1024px) {
            .left-side {
                display: flex;
                align-items: center;
                justify-content: center;
            }

            .right-side {
                width: 50%;
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .login-form {
            animation: fadeInUp 0.5s ease-out;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="left-side">
            <div>
                <h1>Welcome Back!</h1>
                <p>We're so excited to see you again!</p>
            </div>
        </div>
        <div class="right-side">
            <div class="login-form">
                <h1>Sign in to your account</h1>
                <form>
                    <div class="form-group">
                        <label for="email-address">Email address</label>
                        <input id="email-address" name="email" type="email" autocomplete="email" required placeholder="Email address">
                    </div>
                    <div class="form-group">
                        <label for="password">Password</label>
                        <input id="password" name="password" type="password" autocomplete="current-password" required placeholder="Password">
                    </div>
                    <button type="submit">Sign in</button>
                </form>
                <p class="signup-link">
                    Don't have an account? <a href="#">Sign up now</a>
                </p>
            </div>
        </div>
    </div>
</body>
</html>
