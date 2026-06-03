<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Pack Pilot – Your Smart Travel Companion</title>
  <link rel="stylesheet" href="style.css" />
  <link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=DM+Sans:ital,wght@0,300;0,400;0,500;1,300&display=swap" rel="stylesheet" />
</head>
<body>

<!-- ========== SCREEN: Login / Sign Up ========== -->
<div id="screen-auth" class="screen active">
  <div class="auth-bg">
    <div class="auth-blob b1"></div>
    <div class="auth-blob b2"></div>
    <div class="auth-blob b3"></div>
  </div>
  <div class="auth-card">
    <div class="logo-mark">✈</div>
    <h1 class="brand">Pack<span>Pilot</span></h1>
    <p class="tagline">Your smart travel packing companion</p>

    <div class="tab-row">
      <button class="tab active" data-tab="login">Log In</button>
      <button class="tab" data-tab="signup">Sign Up</button>
    </div>

    <!-- Login -->
    <div id="tab-login" class="tab-panel active">
      <div class="field-group">
        <label>Email</label>
        <input type="email" id="login-email" placeholder="you@example.com" />
      </div>
      <div class="field-group">
        <label>Password</label>
        <input type="password" id="login-password" placeholder="••••••••" />
      </div>
      <button class="btn-primary full" onclick="doLogin()">Log In</button>
      <p class="switch-text">Don't have an account? <a href="#" onclick="switchTab('signup')">Sign up</a></p>
    </div>

    <!-- Sign Up -->
    <div id="tab-signup" class="tab-panel">
      <div class="field-group">
        <label>Name</label>
        <input type="text" id="signup-name" placeholder="Your name" />
      </div>
      <div class="field-group">
        <label>Email</label>
        <input type="email" id="signup-email" placeholder="you@example.com" />
      </div>
      <div class="field-group">
        <label>Password</label>
        <input type="password" id="signup-password" placeholder="Create password" />
      </div>
      <div class="field-group">
        <label>Date of Birth</label>
        <input type="date" id="signup-dob" />
      </div>
      <button class="btn-primary full" onclick="doSignup()">Create Account</button>
      <p class="switch-text">Already have an account? <a href="#" onclick="switchTab('login')">Log in</a></p>
    </div>
  </div>
</div>
