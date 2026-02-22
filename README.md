<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Sign Up – JLM RYAN Tech</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <main class="signup-root">
    <section class="form-wrap">

      <div class="brand">
        <h1>Sign Up to JLM RYAN'S</h1>
        <p class="tag">For Exclusive Content -- join JLM RYAN'S Tech</p>
      </div>

      <!-- Signup Form -->
      <form id="signup-form" class="signup-form" novalidate>

        <div class="field">
          <label for="name">Full name</label>
          <input
            id="name"
            name="name"
            type="text"
            placeholder="Enter your full name"
            required
            autocomplete="name"
          />
        </div>

        <div class="field">
          <label for="email">Email</label>
          <input
            id="email"
            name="email"
            type="email"
            placeholder="your.email@example.com"
            required
            autocomplete="email"
          />
        </div>

        <!-- Password -->
        <div class="field">
          <label for="password">Password</label>
          <div class="input-with-icon">
            <input
              id="password"
              name="password"
              type="password"
              placeholder="Enter a password"
              minlength="6"
              required
              autocomplete="new-password"
            />
            <button
              type="button"
              class="pw-toggle"
              id="pw-toggle"
              aria-label="Show password"
            >
              👁
            </button>
          </div>

          <div class="strength" aria-hidden="true">
            <div class="strength-bar" id="strength-bar"></div>
          </div>
        </div>

        <div class="field">
          <label for="confirm">Confirm password</label>
          <input
            id="confirm"
            name="confirm"
            type="password"
            placeholder="Confirm your password"
            minlength="6"
            required
            autocomplete="new-password"
          />
        </div>

        <button type="submit" class="btn-primary">Create Account</button>

      </form>
    </section>
  </main>

<script>
  const toggle = document.getElementById("pw-toggle");
  const password = document.getElementById("password");

  toggle.addEventListener("click", () => {
    password.type = password.type === "password" ? "text" : "password";
  });
</script>

</body>
</html># Ryan-MJ-
