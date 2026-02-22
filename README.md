<!DOCTYPE html>

<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>HonorPay — Veteran Financial Services</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet"/>
  <style>
    :root {
      --navy: #0d1f3c;
      --navy-mid: #162847;
      --navy-light: #1e3660;
      --grey-dark: #2c3444;
      --grey-mid: #5a6478;
      --grey-light: #9aa0ad;
      --grey-pale: #e4e8ef;
      --white: #ffffff;
      --bg: #f4f6fa;
      --accent: #1a4a8a;
      --accent-hover: #153d74;
      --border: #d2d7e0;
      --gold: #b8922a;
      --gold-light: #f5ecd4;
    }

```
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
  background: var(--bg);
  font-family: 'Inter', sans-serif;
  color: var(--navy);
  line-height: 1.6;
}

/* ────────────────── TOP BAR ────────────────── */
.topbar {
  background: var(--navy);
  padding: 0 60px;
  height: 68px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.brand {
  display: flex;
  align-items: center;
  gap: 12px;
  text-decoration: none;
}

.brand-icon {
  width: 34px;
  height: 34px;
  background: var(--gold);
  border-radius: 4px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.brand-icon svg {
  width: 18px;
  height: 18px;
  fill: white;
}

.brand-name {
  font-family: 'Playfair Display', serif;
  font-size: 21px;
  color: var(--white);
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 32px;
}

.nav-links a {
  font-size: 13.5px;
  color: var(--grey-light);
  text-decoration: none;
  font-weight: 400;
  transition: color 0.15s;
}

.nav-links a:hover { color: var(--white); }

.nav-links .nav-cta {
  background: var(--gold);
  color: var(--white);
  padding: 8px 20px;
  border-radius: 4px;
  font-weight: 600;
  font-size: 13px;
}

.nav-links .nav-cta:hover { background: #a07b22; color: var(--white); }

/* ────────────────── HERO / INTRO ────────────────── */
.hero {
  background: var(--navy-mid);
  padding: 72px 60px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 60px;
  border-bottom: 3px solid var(--gold);
}

.hero-text {
  max-width: 520px;
}

.eyebrow {
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 16px;
}

.hero-text h1 {
  font-family: 'Playfair Display', serif;
  font-size: 38px;
  color: var(--white);
  line-height: 1.25;
  margin-bottom: 20px;
}

.hero-text p {
  font-size: 15px;
  color: var(--grey-light);
  line-height: 1.8;
  font-weight: 300;
}

/* ────────────────── LOGIN CARD ────────────────── */
.login-card {
  background: var(--white);
  border-radius: 8px;
  border: 1px solid var(--border);
  width: 100%;
  max-width: 400px;
  flex-shrink: 0;
  overflow: hidden;
}

.login-card-header {
  background: var(--navy);
  padding: 24px 32px;
  border-bottom: 2px solid var(--gold);
}

.login-card-header h2 {
  font-family: 'Playfair Display', serif;
  font-size: 20px;
  color: var(--white);
}

.login-card-header p {
  font-size: 13px;
  color: var(--grey-light);
  margin-top: 4px;
}

.login-card-body {
  padding: 28px 32px 32px;
}

.form-group {
  margin-bottom: 18px;
}

.form-group label {
  display: block;
  font-size: 12px;
  font-weight: 600;
  letter-spacing: 0.4px;
  color: var(--grey-dark);
  margin-bottom: 7px;
  text-transform: uppercase;
}

.form-group input {
  width: 100%;
  padding: 11px 13px;
  border: 1px solid var(--border);
  border-radius: 5px;
  font-family: 'Inter', sans-serif;
  font-size: 14px;
  color: var(--navy);
  outline: none;
  transition: border-color 0.2s, box-shadow 0.2s;
}

.form-group input:focus {
  border-color: var(--accent);
  box-shadow: 0 0 0 3px rgba(26,74,138,0.09);
}

.form-row {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 22px;
}

.check-label {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 13px;
  color: var(--grey-mid);
  cursor: pointer;
}

.check-label input { accent-color: var(--accent); width: 14px; height: 14px; }

.forgot { font-size: 13px; color: var(--accent); text-decoration: none; font-weight: 500; }
.forgot:hover { text-decoration: underline; }

.btn-primary {
  width: 100%;
  padding: 13px;
  background: var(--accent);
  color: var(--white);
  border: none;
  border-radius: 5px;
  font-family: 'Inter', sans-serif;
  font-size: 14px;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.2s;
}

.btn-primary:hover { background: var(--accent-hover); }

.sep {
  display: flex;
  align-items: center;
  gap: 10px;
  margin: 16px 0;
}

.sep hr { flex: 1; border: none; border-top: 1px solid var(--border); }
.sep span { font-size: 12px; color: var(--grey-light); }

.btn-outline {
  width: 100%;
  padding: 11px;
  background: transparent;
  color: var(--accent);
  border: 1px solid var(--accent);
  border-radius: 5px;
  font-family: 'Inter', sans-serif;
  font-size: 14px;
  font-weight: 500;
  cursor: pointer;
  transition: background 0.15s;
}

.btn-outline:hover { background: rgba(26,74,138,0.05); }

/* ────────────────── SERVICES SECTION ────────────────── */
.services-section {
  padding: 80px 60px;
  background: var(--white);
}

.section-header {
  margin-bottom: 56px;
}

.section-header .eyebrow {
  color: var(--gold);
}

.section-header h2 {
  font-family: 'Playfair Display', serif;
  font-size: 30px;
  color: var(--navy);
  margin-bottom: 12px;
}

.section-header p {
  font-size: 15px;
  color: var(--grey-mid);
  max-width: 540px;
  line-height: 1.75;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 2px;
  background: var(--border);
  border: 1px solid var(--border);
  border-radius: 8px;
  overflow: hidden;
}

.service-card {
  background: var(--white);
  padding: 44px 40px;
  position: relative;
}

.service-number {
  font-family: 'Playfair Display', serif;
  font-size: 48px;
  color: var(--grey-pale);
  font-weight: 700;
  line-height: 1;
  margin-bottom: 20px;
}

.service-card h3 {
  font-size: 17px;
  font-weight: 600;
  color: var(--navy);
  margin-bottom: 12px;
  line-height: 1.3;
}

.service-card p {
  font-size: 14px;
  color: var(--grey-mid);
  line-height: 1.75;
}

.service-tag {
  display: inline-block;
  margin-top: 20px;
  padding: 5px 12px;
  background: var(--gold-light);
  color: var(--gold);
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.5px;
  border-radius: 3px;
  text-transform: uppercase;
}

/* ────────────────── HOW IT WORKS ────────────────── */
.process-section {
  padding: 80px 60px;
  background: var(--bg);
}

.steps {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0;
  margin-top: 48px;
  position: relative;
}

.steps::before {
  content: '';
  position: absolute;
  top: 22px;
  left: calc(12.5% + 16px);
  right: calc(12.5% + 16px);
  height: 1px;
  background: var(--border);
  z-index: 0;
}

.step {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding: 0 16px;
  position: relative;
  z-index: 1;
}

.step-num {
  width: 44px;
  height: 44px;
  background: var(--navy);
  color: var(--white);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 14px;
  font-weight: 600;
  margin-bottom: 20px;
  flex-shrink: 0;
}

.step h4 {
  font-size: 14px;
  font-weight: 600;
  color: var(--navy);
  margin-bottom: 8px;
}

.step p {
  font-size: 13px;
  color: var(--grey-mid);
  line-height: 1.65;
}

/* ────────────────── COMPLIANCE SECTION ────────────────── */
.compliance-section {
  background: var(--navy);
  padding: 60px;
  display: flex;
  gap: 80px;
  align-items: flex-start;
}

.compliance-block {
  flex: 1;
}

.compliance-block .eyebrow {
  color: var(--gold);
  margin-bottom: 14px;
}

.compliance-block h3 {
  font-family: 'Playfair Display', serif;
  font-size: 20px;
  color: var(--white);
  margin-bottom: 16px;
}

.compliance-block p {
  font-size: 13.5px;
  color: var(--grey-light);
  line-height: 1.8;
}

.compliance-block a {
  color: var(--grey-pale);
  text-decoration: underline;
}

.compliance-divider {
  width: 1px;
  background: rgba(255,255,255,0.1);
  align-self: stretch;
}

.compliance-badges {
  display: flex;
  flex-direction: column;
  gap: 14px;
  min-width: 220px;
}

.badge {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 14px 16px;
  background: rgba(255,255,255,0.05);
  border: 1px solid rgba(255,255,255,0.08);
  border-radius: 5px;
}

.badge-icon {
  width: 28px;
  height: 28px;
  background: var(--gold);
  border-radius: 4px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}

.badge-icon svg { width: 14px; height: 14px; fill: white; }

.badge-text {
  font-size: 12.5px;
  color: var(--grey-pale);
  font-weight: 500;
}

/* ────────────────── FOOTER ────────────────── */
.footer {
  background: var(--navy-mid);
  padding: 24px 60px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-top: 1px solid rgba(255,255,255,0.07);
}

.footer p {
  font-size: 12.5px;
  color: var(--grey-mid);
}

.footer-links {
  display: flex;
  gap: 24px;
}

.footer-links a {
  font-size: 12.5px;
  color: var(--grey-light);
  text-decoration: none;
}

.footer-links a:hover { color: var(--white); }

/* ────────────────── RESPONSIVE ────────────────── */
@media (max-width: 960px) {
  .hero { flex-direction: column; padding: 48px 32px; }
  .login-card { max-width: 100%; }
  .services-grid { grid-template-columns: 1fr; }
  .steps { grid-template-columns: repeat(2, 1fr); }
  .steps::before { display: none; }
  .compliance-section { flex-direction: column; gap: 40px; padding: 48px 32px; }
  .compliance-divider { display: none; }
  .topbar, .services-section, .process-section, .footer { padding-left: 32px; padding-right: 32px; }
}

@media (max-width: 600px) {
  .nav-links { display: none; }
  .steps { grid-template-columns: 1fr; }
}
```

  </style>
</head>
<body>

  <!-- Top Bar -->

  <header class="topbar">
    <a href="#" class="brand">
      <div class="brand-icon">
        <svg viewBox="0 0 24 24"><path d="M12 2L3 7v5c0 5.25 3.75 10.15 9 11.35C17.25 22.15 21 17.25 21 12V7L12 2z"/></svg>
      </div>
      <span class="brand-name">HonorPay</span>
    </a>
    <nav class="nav-links">
      <a href="#services">Services</a>
      <a href="#how-it-works">How It Works</a>
      <a href="#compliance">Compliance</a>
      <a href="#" class="nav-cta">Sign In</a>
    </nav>
  </header>

  <!-- Hero + Login -->

  <section class="hero">
    <div class="hero-text">
      <div class="eyebrow">Veteran Financial Services</div>
      <h1>Your Benefits.<br/>Your Rights.<br/>Our Process.</h1>
      <p>
        HonorPay helps veterans and their families navigate the financial benefits they've earned —
        with clear guidance, professional documentation support, and transparent processing at every step.
      </p>
    </div>

```
<div class="login-card">
  <div class="login-card-header">
    <h2>Access Your Account</h2>
    <p>Sign in to manage your case and documents.</p>
  </div>
  <div class="login-card-body">
    <form onsubmit="return false;">
      <div class="form-group">
        <label for="email">Email Address</label>
        <input type="email" id="email" placeholder="you@example.com" autocomplete="email"/>
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" id="password" placeholder="••••••••" autocomplete="current-password"/>
      </div>
      <div class="form-row">
        <label class="check-label">
          <input type="checkbox"/> Keep me signed in
        </label>
        <a href="#" class="forgot">Forgot password?</a>
      </div>
      <button type="submit" class="btn-primary">Sign In to My Account</button>
      <div class="sep"><hr/><span>New to HonorPay?</span><hr/></div>
      <button type="button" class="btn-outline">Create an Account</button>
    </form>
  </div>
</div>
```

  </section>

  <!-- Services -->

  <section class="services-section" id="services">
    <div class="section-header">
      <div class="eyebrow">What We Do</div>
      <h2>Our Core Services</h2>
      <p>We provide focused, professional support across four areas of veteran financial processing. No upsells. No vague promises.</p>
    </div>

```
<div class="services-grid">

  <div class="service-card">
    <div class="service-number">01</div>
    <h3>Benefit Review &amp; Eligibility Assessment</h3>
    <p>
      We conduct a thorough review of your service record, discharge status, and existing claims
      to identify benefits you may be entitled to under current VA and federal guidelines.
      You receive a clear, written summary of your eligibility profile.
    </p>
    <span class="service-tag">Assessment</span>
  </div>

  <div class="service-card">
    <div class="service-number">02</div>
    <h3>Fund Retrieval Assistance</h3>
    <p>
      For veterans with approved or pending benefit awards, we assist in tracking outstanding
      payments, identifying processing delays, and coordinating with the appropriate agencies
      to move your case forward through proper channels.
    </p>
    <span class="service-tag">Financial</span>
  </div>

  <div class="service-card">
    <div class="service-number">03</div>
    <h3>Documentation Support</h3>
    <p>
      Incomplete or improperly submitted documentation is among the most common reasons
      benefit claims are delayed or denied. We help you compile, format, and submit
      the right records to support your case from the start.
    </p>
    <span class="service-tag">Documentation</span>
  </div>

  <div class="service-card">
    <div class="service-number">04</div>
    <h3>Post-Service Financial Processing</h3>
    <p>
      We support veterans transitioning out of active duty in understanding separation pay,
      retirement processing, survivor benefit options, and other financial obligations
      that arise at the end of military service.
    </p>
    <span class="service-tag">Transition</span>
  </div>

</div>
```

  </section>

  <!-- How It Works -->

  <section class="process-section" id="how-it-works">
    <div class="section-header">
      <div class="eyebrow">The Process</div>
      <h2>How It Works</h2>
      <p>A straightforward four-step process designed around your situation — not a one-size-fits-all template.</p>
    </div>

```
<div class="steps">
  <div class="step">
    <div class="step-num">1</div>
    <h4>Submit Your Information</h4>
    <p>Create a secure account and provide your service and benefit background.</p>
  </div>
  <div class="step">
    <div class="step-num">2</div>
    <h4>Eligibility Review</h4>
    <p>Our team reviews your profile and identifies applicable benefit programs.</p>
  </div>
  <div class="step">
    <div class="step-num">3</div>
    <h4>Document &amp; File</h4>
    <p>We assist in preparing and submitting the required documentation.</p>
  </div>
  <div class="step">
    <div class="step-num">4</div>
    <h4>Track &amp; Follow Up</h4>
    <p>We monitor your case status and follow up with agencies on your behalf.</p>
  </div>
</div>
```

  </section>

  <!-- Compliance -->

  <section class="compliance-section" id="compliance">

```
<div class="compliance-block">
  <div class="eyebrow">Legal &amp; Regulatory</div>
  <h3>Our Compliance Commitment</h3>
  <p>
    HonorPay operates in accordance with VA regulations, the Veterans Benefits Act,
    and all applicable federal and state financial services laws. We do not charge
    fees for initial benefit reviews. All service agreements are provided in writing
    prior to engagement. We are not affiliated with the Department of Veterans Affairs.
  </p>
</div>

<div class="compliance-divider"></div>

<div class="compliance-block">
  <div class="eyebrow">Data &amp; Privacy</div>
  <h3>Your Information Is Protected</h3>
  <p>
    All data submitted through this portal is encrypted in transit and at rest.
    Your records are never sold or shared with third parties without your written consent.
    You may request deletion of your account and all associated data at any time.
    See our full <a href="#">Privacy Policy</a> and <a href="#">Terms of Service</a>.
  </p>
</div>

<div class="compliance-divider"></div>

<div class="compliance-badges">
  <div class="badge">
    <div class="badge-icon">
      <svg viewBox="0 0 24 24"><path d="M12 2L3 7v5c0 5.25 3.75 10.15 9 11.35C17.25 22.15 21 17.25 21 12V7L12 2z"/></svg>
    </div>
    <span class="badge-text">256-bit SSL Encryption</span>
  </div>
  <div class="badge">
    <div class="badge-icon">
      <svg viewBox="0 0 24 24"><path d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"/></svg>
    </div>
    <span class="badge-text">Regulated Financial Services</span>
  </div>
  <div class="badge">
    <div class="badge-icon">
      <svg viewBox="0 0 24 24"><path d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z"/></svg>
    </div>
    <span class="badge-text">Sessions Monitored &amp; Logged</span>
  </div>
</div>
```

  </section>

  <!-- Footer -->

  <footer class="footer">
    <p>© 2025 HonorPay Financial Services. All rights reserved. Not affiliated with the U.S. Department of Veterans Affairs.</p>
    <div class="footer-links">
      <a href="#">Privacy Policy</a>
      <a href="#">Terms of Service</a>
      <a href="#">Accessibility</a>
      <a href="#">Contact</a>
    </div>
  </footer>

</body>
</html>
