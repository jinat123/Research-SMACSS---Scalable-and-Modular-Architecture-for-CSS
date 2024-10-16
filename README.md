<!DOCTYPE html>
<html lang="">
<html lang="en">
<head>
  <title>SMACSS Example</title>
  <link rel="stylesheet" href="index.css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="index.css">
    <title>SMACSS Example</title>
</head>
<body>
  <div class="container">
    <h1>Welcome to SMACSS</h1>
    <p>This is a simple example of a webpage built using SMACSS principles.</p>
    <button class="button button--primary">Learn More</button>
  </div>
    <header class="site-header">
        <h1>Welcome to SMACSS Example</h1>
        <nav class="site-nav">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section class="card">
            <h2 class="card-title">Card Title 1</h2>
            <p class="card-description">This is a reusable card component based on SMACSS principles.</p>
        </section>
        <section class="card card--active">
            <h2 class="card-title">Card Title 2</h2>
            <p class="card-description">Another instance of a card component in an active state.</p>
        </section>
    </main>
    <footer class="site-footer">
        <p>© 2024 Jinelyn Mangubat</p>
    </footer>
</body>
</html>




/* Base */
body {
  font-family: sans-serif;
  margin: 0;
    font-family: Arial, sans-serif;
    background-color: #f7f7f7;
    margin: 0;
    padding: 0;
}

h1 {
    font-size: 2em;
    margin-bottom: 1em;
    /* Layout */

    .site-header, .site-footer {
        background-color: #333;
        color: #fff;
        text-align: center;
        padding: 20px 0;
    }

    p {
        line-height: 1.5;

        .site-header h1 {
            margin: 0;
        }

        /* Layout */

        .container {
            max-width: 960px;
            margin: 0 auto;
            padding: 20px;

            .site-nav ul {
                list-style: none;
                padding: 0;
                margin: 0;
                display: flex;
                justify-content: center;
            }

            .site-nav li {
                margin: 0 15px;
            }

            .site-nav a {
                color: #fff;
                text-decoration: none;
            }

            .site-footer {
                font-size: 0.9em;
                margin-top: 20px;
            }

            /* Module */

            .button {
                padding: 10px 20px;
                border: none;
                border-radius: 5px;
                cursor: pointer;

                .card {
                    background-color: #fff;
                    border-radius: 5px;
                    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
                    padding: 20px;
                    margin: 20px auto;
                    width: 90%;
                    max-width: 800px;
                }

                .card--active {
                    border: 2px solid #007bff;
                }

                /* State */

                .button--primary {
                    background-color: #007bff;
                    color: #fff;

                    .card-title {
                        margin: 0;
                        font-size: 1.5em;
                    }

                    /* Theme */

                    body {
                        background-color: #f0f0f0;

                        .card-description {
                            font-size: 1em;
                            color: #555;
                        }
                    }
                }
            }
        }
    }
}
