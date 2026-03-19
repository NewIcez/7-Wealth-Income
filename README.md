
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>7 Income Streams – Dark Mode</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@700;800&family=Epilogue:wght@400;500;700;900&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: #15202b;
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    padding: 40px 20px;
    font-family: 'Epilogue', sans-serif;
  }

  .card {
    width: 560px;
    background: #ffffff;
    border-radius: 16px;
    overflow: hidden;
    position: relative;
  }

  /* Loud top accent */
  .top-accent {
    height: 8px;
    background: #00e5a0;
    width: 100%;
  }

  /* Hero block */
  .hero {
    background: #0a0a0a;
    padding: 36px 40px 32px;
    position: relative;
    overflow: hidden;
  }

  /* Giant ghost number */
  .ghost {
    position: absolute;
    right: -16px;
    top: -24px;
    font-family: 'Syne', sans-serif;
    font-size: 200px;
    font-weight: 800;
    color: rgba(255,255,255,0.04);
    line-height: 1;
    user-select: none;
    pointer-events: none;
  }

  .tag {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    border: 1px solid rgba(0,229,160,0.35);
    color: #00e5a0;
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 2.5px;
    text-transform: uppercase;
    padding: 5px 12px;
    border-radius: 100px;
    margin-bottom: 20px;
  }

  .tag-dot {
    width: 5px; height: 5px;
    background: #00e5a0;
    border-radius: 50%;
    animation: pulse 2s ease-in-out infinite;
  }

  @keyframes pulse {
    0%,100% { opacity: 1; transform: scale(1); }
    50% { opacity: 0.5; transform: scale(0.7); }
  }

  .hero-heading {
    font-family: 'Syne', sans-serif;
    font-size: 38px;
    font-weight: 800;
    color: #ffffff;
    line-height: 1.08;
    letter-spacing: -0.5px;
  }

  .hero-heading .accent { color: #00e5a0; }

  .hero-sub {
    margin-top: 12px;
    font-size: 13px;
    color: rgba(255,255,255,0.35);
    line-height: 1.6;
    font-weight: 400;
  }

  /* Stream rows */
  .streams {
    background: #ffffff;
    padding: 8px 0 0;
  }

  .stream {
    display: grid;
    grid-template-columns: 56px 1fr 82px;
    align-items: center;
    gap: 0 12px;
    padding: 15px 28px;
    border-bottom: 1px solid #f0f0f0;
    position: relative;
  }

  .stream:last-child { border-bottom: none; }

  /* Left number */
  .num {
    font-family: 'Syne', sans-serif;
    font-size: 13px;
    font-weight: 800;
    color: #d0d0d0;
    letter-spacing: 0.5px;
  }

  /* Title + desc */
  .stream-name {
    font-family: 'Syne', sans-serif;
    font-size: 15px;
    font-weight: 800;
    color: #0a0a0a;
    letter-spacing: -0.2px;
    margin-bottom: 2px;
  }

  .stream-desc {
    font-size: 11px;
    color: #888;
    font-weight: 400;
    line-height: 1.5;
  }

  /* Type badge */
  .badge {
    font-size: 9px;
    font-weight: 700;
    letter-spacing: 1.5px;
    text-transform: uppercase;
    padding: 4px 10px;
    border-radius: 100px;
    text-align: center;
    white-space: nowrap;
    justify-self: end;
  }

  .b-active    { background: #fff8e6; color: #b07800; }
  .b-passive   { background: #e6faf4; color: #007a55; }
  .b-portfolio { background: #eef2ff; color: #3a5bbf; }

  /* Bottom bar */
  .bottom {
    background: #0a0a0a;
    padding: 20px 28px 24px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 16px;
  }

  .bottom-stat {
    display: flex;
    align-items: baseline;
    gap: 10px;
  }

  .stat-big {
    font-family: 'Syne', sans-serif;
    font-size: 48px;
    font-weight: 800;
    color: #00e5a0;
    line-height: 1;
  }

  .stat-copy {
    font-size: 12px;
    color: rgba(255,255,255,0.4);
    line-height: 1.5;
    max-width: 120px;
  }

  .stat-copy strong {
    display: block;
    color: rgba(255,255,255,0.85);
    font-size: 13px;
    font-weight: 700;
    margin-bottom: 2px;
  }

  .cta-right {
    text-align: right;
  }

  .cta-question {
    font-size: 12px;
    color: rgba(255,255,255,0.45);
    margin-bottom: 10px;
    line-height: 1.4;
  }

  .cta-question strong {
    color: #ffffff;
    display: block;
    font-size: 13px;
    font-weight: 700;
    margin-bottom: 2px;
  }

  .cta-btn {
    display: inline-block;
    background: #00e5a0;
    color: #0a0a0a;
    font-family: 'Syne', sans-serif;
    font-size: 11px;
    font-weight: 800;
    letter-spacing: 2px;
    text-transform: uppercase;
    padding: 10px 20px;
    border-radius: 100px;
  }

  /* Bottom accent */
  .bottom-accent {
    height: 4px;
    background: repeating-linear-gradient(
      90deg,
      #00e5a0 0px, #00e5a0 24px,
      #0a0a0a 24px, #0a0a0a 26px
    );
  }
</style>
</head>
<body>
<div class="card">

  <div class="top-accent"></div>

  <div class="hero">
    <div class="ghost">7</div>
    <div class="tag">
      <div class="tag-dot"></div>
      Financial literacy
    </div>
    <div class="hero-heading">
      The average millionaire<br>
      has <span class="accent">7 income streams.</span><br>
      You were taught<br>to get 1 job.
    </div>
    <div class="hero-sub">
      Here are all 7 — and which ones to start building first.
    </div>
  </div>

  <div class="streams">

    <div class="stream">
      <div class="num">01</div>
      <div>
        <div class="stream-name">Earned Income</div>
        <div class="stream-desc">Salary or freelance. Fund everything else from here.</div>
      </div>
      <div class="badge b-active">Active</div>
    </div>

    <div class="stream">
      <div class="num">02</div>
      <div>
        <div class="stream-name">Business Income</div>
        <div class="stream-desc">Revenue from a business you own. Biggest upside.</div>
      </div>
      <div class="badge b-active">Active</div>
    </div>

    <div class="stream">
      <div class="num">03</div>
      <div>
        <div class="stream-name">Interest Income</div>
        <div class="stream-desc">Savings, bonds, or lending. Low effort, steady return.</div>
      </div>
      <div class="badge b-passive">Passive</div>
    </div>

    <div class="stream">
      <div class="num">04</div>
      <div>
        <div class="stream-name">Dividend Income</div>
        <div class="stream-desc">Stocks that pay you quarterly just for holding.</div>
      </div>
      <div class="badge b-portfolio">Portfolio</div>
    </div>

    <div class="stream">
      <div class="num">05</div>
      <div>
        <div class="stream-name">Rental Income</div>
        <div class="stream-desc">Tenant covers mortgage. You keep the upside.</div>
      </div>
      <div class="badge b-passive">Passive</div>
    </div>

    <div class="stream">
      <div class="num">06</div>
      <div>
        <div class="stream-name">Capital Gains</div>
        <div class="stream-desc">Profit from selling assets — stocks, property, crypto.</div>
      </div>
      <div class="badge b-portfolio">Portfolio</div>
    </div>

    <div class="stream">
      <div class="num">07</div>
      <div>
        <div class="stream-name">Royalty Income</div>
        <div class="stream-desc">Paid forever for work done once. Books, products, IP.</div>
      </div>
      <div class="badge b-passive">Passive</div>
    </div>

  </div>

  <div class="bottom">
    <div class="bottom-stat">
      <div class="stat-big">7</div>
      <div class="stat-copy">
        <strong>streams.</strong>
        Most people never get past 1.
      </div>
    </div>
    <div class="cta-right">
      <div class="cta-question">
        <strong>Which are you building?</strong>
        Drop the number below ↓
      </div>
      <div class="cta-btn">Comment</div>
    </div>
  </div>

  <div class="bottom-accent"></div>

</div>
</body>
</html>
