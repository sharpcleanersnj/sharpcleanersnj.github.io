---
layout: page
title: Contact
permalink: /contact/
---

<style>
  .contact-page {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    color: #0f172a;
  }

  .contact-inner {
    max-width: 1100px;
    margin: 0 auto;
    padding: 2.5rem 1.5rem 3.5rem;
  }

  .contact-header {
    text-align: center;
    margin-bottom: 2.25rem;
  }

  .contact-header h1 {
    margin: 0 0 0.4rem;
    font-size: clamp(2rem, 3vw, 2.5rem);
    letter-spacing: 0.06em;
    text-transform: uppercase;
  }

  .contact-tagline {
    margin: 0;
    font-size: 0.98rem;
    color: #6b7280;
  }

  .contact-layout {
    display: grid;
    grid-template-columns: minmax(0, 1.2fr) minmax(0, 1.1fr);
    gap: 2rem;
    align-items: flex-start;
  }

  /* FORM */

  .contact-card {
    background: #ffffff;
    border-radius: 0.9rem;
    padding: 1.75rem 1.5rem 1.9rem;
    border: 1px solid #e5e7eb;
    box-shadow: 0 10px 26px rgba(15, 23, 42, 0.08);
  }

  .contact-card h2 {
    margin-top: 0;
    margin-bottom: 0.4rem;
    font-size: 1.25rem;
  }

  .contact-card p {
    margin-top: 0;
    margin-bottom: 1.3rem;
    font-size: 0.95rem;
    color: #6b7280;
  }

  .contact-form-row {
    margin-bottom: 0.9rem;
  }

  .contact-form-row label {
    display: block;
    font-size: 0.84rem;
    text-transform: uppercase;
    letter-spacing: 0.16em;
    font-weight: 600;
    color: #6b7280;
    margin-bottom: 0.3rem;
  }

  .contact-form-row input,
  .contact-form-row select,
  .contact-form-row textarea {
    width: 100%;
    font-size: 0.95rem;
    padding: 0.55rem 0.6rem;
    border-radius: 0.55rem;
    border: 1px solid #d1d5db;
    background: #f9fafb;
    transition: border-color 0.15s ease, box-shadow 0.15s ease, background-color 0.15s ease;
  }

  .contact-form-row input:focus,
  .contact-form-row select:focus,
  .contact-form-row textarea:focus {
    outline: none;
    border-color: #2563eb;
    box-shadow: 0 0 0 1px #2563eb33;
    background: #ffffff;
  }

  .contact-form-row textarea {
    min-height: 130px;
    resize: vertical;
  }

  .contact-helper {
    font-size: 0.8rem;
    color: #9ca3af;
    margin-top: 0.2rem;
  }

  .contact-submit {
    margin-top: 1rem;
  }

  .contact-submit button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    padding: 0.7rem 1.7rem;
    border-radius: 999px;
    border: none;
    font-size: 0.92rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.18em;
    background: #2563eb;
    color: #ffffff;
    cursor: pointer;
    box-shadow: 0 12px 30px rgba(37, 99, 235, 0.45);
    transition: background-color 0.15s ease, transform 0.12s ease, box-shadow 0.15s ease;
  }

  .contact-submit button:hover {
    background-color: #1d4ed8;
    transform: translateY(-1px);
    box-shadow: 0 14px 34px rgba(37, 99, 235, 0.55);
  }

  .contact-submit button:active {
    transform: translateY(0);
    box-shadow: 0 8px 20px rgba(37, 99, 235, 0.4);
  }

  /* LOCATIONS SIDEBAR */

  .locations-card {
    background: #0f172a;
    border-radius: 0.9rem;
    padding: 1.6rem 1.45rem 1.9rem;
    color: #e5e7eb;
    border: 1px solid #1e293b;
    box-shadow: 0 10px 26px rgba(15, 23, 42, 0.9);
  }

  .locations-card h2 {
    margin-top: 0;
    margin-bottom: 0.3rem;
    font-size: 1.2rem;
  }

  .locations-card p {
    margin-top: 0;
    margin-bottom: 1rem;
    font-size: 0.9rem;
    color: #9ca3af;
  }

  .location-list {
    display: grid;
    grid-template-columns: 1fr;
    gap: 0.8rem;
    font-size: 0.86rem;
  }

  .location-item {
    padding-bottom: 0.7rem;
    border-bottom: 1px solid rgba(148, 163, 184, 0.5);
  }

  .location-item:last-child {
    border-bottom: none;
    padding-bottom: 0;
  }

  .location-name {
    font-weight: 700;
    font-size: 0.98rem;
    margin-bottom: 0.1rem;
  }

  .location-type {
    text-transform: uppercase;
    letter-spacing: 0.16em;
    font-size: 0.76rem;
    color: #a5b4fc;
    margin-bottom: 0.2rem;
  }

  .location-meta span {
    display: block;
  }

  .location-phone a {
    color: #bfdbfe;
    text-decoration: none;
    font-weight: 600;
  }

  .location-phone a:hover {
    text-decoration: underline;
  }

  .location-hours-title {
    margin-top: 0.3rem;
    font-size: 0.78rem;
    text-transform: uppercase;
    letter-spacing: 0.16em;
    color: #9ca3af;
  }

  .location-hours {
    font-size: 0.82rem;
    line-height: 1.3;
  }

  .location-hours span {
    display: block;
  }

  .location-hours .closed {
    color: #fecaca;
    font-weight: 600;
  }

  .contact-social {
    margin-top: 1.1rem;
    font-size: 0.86rem;
  }

  .contact-social a {
    color: #bfdbfe;
    text-decoration: none;
    font-weight: 600;
  }

  .contact-social a:hover {
    text-decoration: underline;
  }

  @media (max-width: 880px) {
    .contact-layout {
      grid-template-columns: minmax(0, 1fr);
    }

    .locations-card {
      order: -1;
    }
  }

  @media (max-width: 640px) {
    .contact-inner {
      padding-inline: 1rem;
      padding-top: 2rem;
    }
  }
</style>

<div class="contact-page">
  <div class="contact-inner">

    <header class="contact-header">
      <h1>Contact Sharp Cleaners</h1>
      <p class="contact-tagline">
        Have a question about dry cleaning, tailoring, or laundry service? We’d love to hear from you.
      </p>
    </header>

    <div class="contact-layout">

      <!-- CONTACT FORM -->
      <section class="contact-card" aria-label="Contact form">
        <h2>Send Us a Message</h2>
        <p>
          Fill out the form below and a member of the Sharp Cleaners team will get back to you as soon as possible.
        </p>

        <form
          method="POST"
          action="https://formspree.io/f/xanvvbja"
        >

          <div class="contact-form-row">
            <label for="name">Your Name *</label>
            <input type="text" id="name" name="name" required />
          </div>

          <div class="contact-form-row">
            <label for="email">Email Address *</label>
            <input type="email" id="email" name="email" required />
          </div>

          <div class="contact-form-row">
            <label for="phone">Phone Number</label>
            <input type="tel" id="phone" name="phone" />
            <div class="contact-helper">Optional, but helpful if we need to reach you quickly.</div>
          </div>

          <div class="contact-form-row">
            <label for="location">Preferred Location</label>
            <select id="location" name="location">
              <option value="">Select a location (optional)</option>
              <option>Northfield</option>
              <option>Ventnor</option>
              <option>Ocean City</option>
              <option>Sea Isle City</option>
              <option>Wildwood</option>
            </select>
          </div>

          <div class="contact-form-row">
            <label for="message">Your Message *</label>
            <textarea id="message" name="message" required></textarea>
          </div>

          <div class="contact-submit">
            <button type="submit">Send Message</button>
          </div>
        </form>
      </section>

      <!-- LOCATIONS & HOURS -->
      <aside class="locations-card" aria-label="Locations and hours">
        <h2>Visit or Call Us</h2>
        <p>
          Prefer to talk in person? Stop by or call any Sharp Cleaners location during business hours.
        </p>

        <div class="location-list">

          <div class="location-item">
            <div class="location-name">Northfield</div>
            <div class="location-type">Dry Cleaners</div>
            <div class="location-meta">
              <span>2327 New Road</span>
              <span>Northfield, NJ 08225</span>
            </div>
            <div class="location-phone">
              <a href="tel:+16094852325">(609) 485-2325</a>
            </div>
            <div class="location-hours-title">Store Hours</div>
            <div class="location-hours">
              <span>Mon – Fri 8:00 AM – 6:00 PM</span>
              <span>Saturday 8:00 AM – 5:00 PM</span>
              <span class="closed">Sunday Closed</span>
            </div>
          </div>

          <div class="location-item">
            <div class="location-name">Ventnor</div>
            <div class="location-type">Dry Cleaners</div>
            <div class="location-meta">
              <span>6519 Ventnor Ave.</span>
              <span>Ventnor, NJ 08406</span>
            </div>
            <div class="location-phone">
              <a href="tel:+16098225866">(609) 822-5866</a>
            </div>
            <div class="location-hours-title">Store Hours</div>
            <div class="location-hours">
              <span>Mon – Sat 9:00 AM – 5:00 PM</span>
              <span class="closed">Sunday Closed</span>
            </div>
          </div>

          <div class="location-item">
            <div class="location-name">Ocean City</div>
            <div class="location-type">Dry Cleaners & Laundromat</div>
            <div class="location-meta">
              <span>121 E. 10th St.</span>
              <span>Ocean City, NJ 08226</span>
            </div>
            <div class="location-phone">
              <a href="tel:+16093997399">(609) 399-7399</a>
            </div>
            <div class="location-hours-title">Dry Cleaners Hours</div>
            <div class="location-hours">
              <span>Mon – Sat 9:00 AM – 5:00 PM</span>
              <span class="closed">Sunday Closed</span>
            </div>
            <div class="location-hours-title">Laundromat Hours</div>
            <div class="location-hours">
              <span>Open 24 Hours</span>
            </div>
          </div>

          <div class="location-item">
            <div class="location-name">Sea Isle City</div>
            <div class="location-type">Dry Cleaners</div>
            <div class="location-meta">
              <span>6216 Landis Ave.</span>
              <span>Sea Isle City, NJ 08243</span>
            </div>
            <div class="location-phone">
              <a href="tel:+16092636400">(609) 263-6400</a>
            </div>
            <div class="location-hours-title">Store Hours</div>
            <div class="location-hours">
              <span>Monday 10:00 AM – 4:00 PM</span>
              <span>Tuesday Closed</span>
              <span>Wednesday 10:00 AM – 4:00 PM</span>
              <span>Thursday Closed</span>
              <span>Friday 10:00 AM – 4:00 PM</span>
              <span>Saturday 10:00 AM – 3:00 PM</span>
              <span class="closed">Sunday Closed</span>
            </div>
          </div>

          <div class="location-item">
            <div class="location-name">Wildwood</div>
            <div class="location-type">Dry Cleaners & Laundromat</div>
            <div class="location-meta">
              <span>3401 New Jersey Ave. #4</span>
              <span>Wildwood, NJ 08260</span>
            </div>
            <div class="location-phone">
              <a href="tel:+16095227719">(609) 522-7719</a>
            </div>
            <div class="location-hours-title">Dry Cleaners Hours</div>
            <div class="location-hours">
              <span>Mononday 10:00 AM – 5:00 PM</span>
              <span>Tuesday Closed</span>
              <span>Wednesday 10:00 AM – 5:00 PM</span>
              <span>Thursday Closed</span>
              <span>Friday 10:00 AM – 5:00 PM</span>
              <span>Saturday 10:00 AM – 4:00 PM</span>
              <span class="closed">Sunday Closed</span>
            </div>
            <div class="location-hours-title">Laundromat Hours</div>
            <div class="location-hours">
              <span>Daily 7:00 AM – 9:00 PM</span>
            </div>
          </div>

        </div>

        <div class="contact-social">
          Connect with us on
          <a href="https://www.facebook.com/sharpcleanersnj/" target="_blank" rel="noopener">Facebook</a>.
        </div>
      </aside>

    </div>
  </div>
</div>
