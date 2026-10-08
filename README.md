# economic-designer-
A platform focused on economic empowerment, personal development, entrepreneurship, and building a community of ambitious individuals committed to creating a better financial future.
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>EDPLAN 3.0 - Sign In</title>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, sans-serif;
  }

  body {
    min-height: 100vh;
    background: linear-gradient(135deg, #4a1a6b 0%, #6b2c91 40%, #8e44ad 100%);
    background-image:
      radial-gradient(circle at 20% 20%, rgba(255,255,255,0.08) 0%, transparent 40%),
      radial-gradient(circle at 80% 70%, rgba(255,255,255,0.06) 0%, transparent 40%),
      linear-gradient(135deg, #3d1554 0%, #5a2280 50%, #7b3fa0 100%);
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 20px;
    position: relative;
    overflow: hidden;
  }

  /* Faint network lines effect */
  body::before {
    content: "";
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(255,255,255,0.05) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255,255,255,0.05) 1px, transparent 1px);
    background-size: 120px 120px;
    opacity: 0.5;
  }

  .container {
    width: 100%;
    max-width: 420px;
    position: relative;
    z-index: 1;
  }

  /* Logo area */
  .logo {
    text-align: center;
    margin-bottom: 25px;
  }

  .logo-ed {
    font-size: 52px;
    font-weight: 900;
    letter-spacing: -2px;
    color: #ffcc33;
    text-shadow: 2px 2px 0 #d68a00, 4px 4px 8px rgba(0,0,0,0.4);
    font-style: italic;
    display: inline-block;
  }

  .logo-ed .d {
    color: #e0e0e0;
    text-shadow: 2px 2px 0 #8a8a8a;
  }

  .logo-plan {
    color: #ffffff;
    font-size: 22px;
    font-weight: 700;
    letter-spacing: 4px;
    margin-top: -5px;
  }

  .logo-sub {
    color: #ffffff;
    font-size: 13px;
    font-weight: 600;
    letter-spacing: 3px;
    margin-top: 4px;
    opacity: 0.9;
  }

  /* Card */
  .card {
    background: #ffffff;
    border-radius: 14px;
    padding: 35px 28px 30px;
    box-shadow: 0 15px 40px rgba(0,0,0,0.35);
  }

  .card h2 {
    text-align: center;
    font-size: 22px;
    color: #222;
    font-weight: 700;
    margin-bottom: 8px;
  }

  .register-line {
    text-align: center;
    font-size: 14px;
    color: #888;
    margin-bottom: 28px;
  }

  .register-line a {
    color: #1a2b8f;
    font-weight: 700;
    text-decoration: none;
  }

  .register-line a:hover {
    text-decoration: underline;
  }

  /* Form fields */
  .field {
    margin-bottom: 20px;
  }

  .field label {
    display: block;
    font-size: 14px;
    font-weight: 600;
    color: #333;
    margin-bottom: 8px;
  }

  .field input {
    width: 100%;
    padding: 13px 14px;
    background: #f4f6fb;
    border: 1px solid #e3e8f0;
    border-radius: 6px;
    font-size: 15px;
    outline: none;
    transition: border 0.2s, background 0.2s;
  }

  .field input:focus {
    border-color: #1a2b8f;
    background: #ffffff;
  }

  /* Button */
  .btn {
    width: 100%;
    padding: 14px;
    background: #152a8f;
    color: #ffffff;
    border: none;
    border-radius: 6px;
    font-size: 16px;
    font-weight: 600;
    cursor: pointer;
    margin-top: 8px;
    transition: background 0.2s, transform 0.1s;
  }

  .btn:hover {
    background: #0f1f70;
  }

  .btn:active {
    transform: scale(0.98);
  }

  @media (max-width: 400px) {
    .logo-ed { font-size: 42px; }
    .card { padding: 28px 20px 24px; }
  }
</style>
</head>
<body>

  <div class="container">

    <!-- Logo -->
    <div class="logo">
      <div class="logo-ed">E<span class="d">D</span></div>
      <div class="logo-plan">PLAN</div>
      <div class="logo-sub">ECONOMY DESIGNER</div>
    </div>

    <!-- Sign-in card -->
    <div class="card">
      <h2>Sign In</h2>
      <p class="register-line">New Here? <a href="#">Register</a></p>

      <form onsubmit="handleLogin(event)">
        <div class="field">
          <label for="username">Username</label>
          <input type="text" id="username" required>
        </div>

        <div class="field">
          <label for="password">Password</label>
          <input type="password" id="password" required>
        </div>

        <button type="submit" class="btn">Continue</button>
      </form>
    </div>

  </div>

  <script>
    function handleLogin(e) {
      e.preventDefault();
      const user = document.getElementById('username').value;
      // This is UI only. Add real login later.
      alert('Login submitted for: ' + user + '\n(No backend connected yet)');
    }
  </script>

</body>
</html>
