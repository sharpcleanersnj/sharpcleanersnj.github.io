---
layout: page
title: Locations & Store Hours
permalink: /locations/
---

<style>
  .locations-page {
    max-width: 1100px;
    margin: 0 auto;
    padding: 1rem 1.5rem 3rem;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  }

  .locations-header {
    text-align: center;
    margin-bottom: 2rem;
  }

  .locations-header h1 {
    font-size: clamp(2rem, 3vw, 2.5rem);
    margin-bottom: 0.25rem;
    letter-spacing: 0.03em;
    text-transform: uppercase;
  }

  .locations-header p {
    margin: 0.25rem 0;
    color: #6b7280;
    font-size: 0.98rem;
  }

  .locations-map {
    margin: 2rem 0 2.5rem;
  }

  .locations-map-inner {
    position: relative;
    padding-top: 56.25%; /* 16:9 ratio */
    border-radius: 0.75rem;
    overflow: hidden;
    box-shadow: 0 10px 25px rgba(15, 23, 42, 0.15);
  }

  .locations-map-inner iframe {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    border: 0;
  }

  .locations-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 1.5rem;
  }

  .location-card {
    background: #ffffff;
    border-radius: 0.75rem;
    padding: 1.5rem 1.25rem;
    box-shadow: 0 4px 14px rgba(15, 23, 42, 0.08);
    border: 1px solid #e5e7eb;
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
  }

  .location-name {
    font-size: 1.25rem;
    font-weight: 700;
    margin-bottom: 0.15rem;
  }

  .location-type {
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    color: #6b7280;
    font-weight: 600;
  }

  .location-type + .location-type {
    margin-left: 0.35rem;
  }

  .location-address {
    font-size: 0.95rem;
    line-height: 1.4;
  }

  .location-address span {
    display: block;
  }

  .location-phone a {
    font-size: 0.95rem;
    font-weight: 600;
    text-decoration: none;
    color: #005a8c;
  }

  .location-phone a:hover {
    text-decoration: underline;
  }

  .hours-block {
    margin-top: 0.5rem;
    border-top: 1px dashed #e5e7eb;
    padding-top: 0.75rem;
  }

  .hours-title {
    font-size: 0.85rem;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    font-weight: 700;
    color: #6b7280;
    margin-bottom: 0.4rem;
  }

  .hours-list {
    font-size: 0.9rem;
    line-height: 1.4;
    display: grid;
    grid-template-columns: 1.3fr 1.7fr;
    column-gap: 0.5rem;
    row-gap: 0.15rem;
  }

  .hours-day {
    font-weight: 500;
  }

  .hours-time {
    color: #111827;
  }

  .closed {
    font-weight: 600;
    color: #b91c1c;
  }

  .location-note {
    font-size: 0.85rem;
    color: #6b7280;
    margin-top: 0.4rem;
  }

  .location-note.important {
    color: #b91c1c;
    font-weight: 600;
  }

  .location-actions {
    margin-top: 0.75rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
  }

  .location-actions a {
    font-size: 0.8rem;
    text-decoration: none;
    padding: 0.35rem 0.75rem;
    border-radius: 999px;
    border: 1px solid #e5e7eb;
    color: #6b7280;
    display: inline-flex;
    align-items: center;
    gap: 0.35rem;
  }

  .location-actions a:hover {
    border-color: #005a8c;
    color: #005a8c;
  }

  @media (max-width: 600px) {
    .locations-page {
      padding-inline: 1rem;
    }

    .locations-map {
      margin: 1.5rem 0 2rem;
    }

    .location-card {
      padding: 1.25rem 1rem;
    }

    .hours-list {
      grid-template-columns: 1.1fr 1.9fr;
    }
  }
</style>

<section class="locations-page">
  <header class="locations-header">
    <h1>Locations &amp; Store Hours</h1>
    <p>Visit any Sharp Cleaners location for professional dry cleaning and laundry services.</p>
    <p>Hours may vary on holidays. Please call to confirm.</p>
  </header>

  <div class="locations-map">
    <div class="locations-map-inner">
      <iframe
        src="https://www.google.com/maps/d/u/0/embed?mid=13szKy6mRagCj-x2ouYiW1ftgoWs&ehbc=2E312F"
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
  </div>

  <div class="locations-grid">

    <!-- Northfield -->
    <article class="location-card" id="northfield">
      <div>
        <div class="location-name">Northfield</div>
        <span class="location-type">Dry Cleaners</span>
      </div>

      <div class="location-address">
        <span>2327 New Road</span>
        <span>Northfield, NJ 08225</span>
      </div>

      <div class="location-phone">
        <a href="tel:+16094852325">(609) 485-2325</a>
      </div>

      <div class="hours-block">
        <div class="hours-title">Store Hours</div>
        <div class="hours-list">
          <span class="hours-day">Monday – Friday</span>
          <span class="hours-time">8:00 AM – 6:00 PM</span>

          <span class="hours-day">Saturday</span>
          <span class="hours-time">8:00 AM – 5:00 PM</span>

          <span class="hours-day">Sunday</span>
          <span class="hours-time closed">Closed</span>
        </div>
      </div>

      <div class="location-actions">
        <a href="https://www.google.com/maps/search/?api=1&query=2327+New+Road,+Northfield,+NJ+08225" target="_blank" rel="noopener">
          <span>📍</span><span>Directions</span>
        </a>
        <a href="tel:+16094852325">
          <span>📞</span><span>Call</span>
        </a>
      </div>
    </article>

    <!-- Ventnor -->
    <article class="location-card" id="ventnor">
      <div>
        <div class="location-name">Ventnor</div>
        <span class="location-type">Dry Cleaners</span>
      </div>

      <div class="location-address">
        <span>6519 Ventnor Ave.</span>
        <span>Ventnor, NJ 08406</span>
      </div>

      <div class="location-phone">
        <a href="tel:+16098225866">(609) 822-5866</a>
      </div>

      <div class="hours-block">
        <div class="hours-title">Store Hours</div>
        <div class="hours-list">
          <span class="hours-day">Monday – Friday</span>
          <span class="hours-time">9:00 AM – 5:00 PM</span>

          <span class="hours-day">Saturday</span>
          <span class="hours-time">10:00 AM – 4:00 PM</span>

          <span class="hours-day">Sunday</span>
          <span class="hours-time closed">Closed</span>
        </div>
      </div>

      <div class="location-actions">
        <a href="https://www.google.com/maps/search/?api=1&query=6519+Ventnor+Ave,+Ventnor,+NJ+08406" target="_blank" rel="noopener">
          <span>📍</span><span>Directions</span>
        </a>
        <a href="tel:+16098225866">
          <span>📞</span><span>Call</span>
        </a>
      </div>
    </article>

    <!-- Ocean City -->
    <article class="location-card" id="ocean-city">
      <div>
        <div class="location-name">Ocean City</div>
        <span class="location-type">Dry Cleaners</span>
      </div>

      <div class="location-address">
        <span>121 E. 10th St.</span>
        <span>Ocean City, NJ 08226</span>
      </div>

      <div class="location-phone">
        <a href="tel:+16093997399">(609) 399-7399</a>
      </div>

      <div class="hours-block">
        <div class="hours-title">Store Hours</div>
        <div class="hours-list">
          <span class="hours-day">Monday – Saturday</span>
          <span class="hours-time">9:00 AM – 5:00 PM</span>

          <span class="hours-day">Sunday</span>
          <span class="hours-time closed">Closed</span>
        </div>
      </div>

      <div class="location-actions">
        <a href="https://www.google.com/maps/search/?api=1&query=121+E+10th+St,+Ocean+City,+NJ+08226" target="_blank" rel="noopener">
          <span>📍</span><span>Directions</span>
        </a>
        <a href="tel:+16093997399">
          <span>📞</span><span>Call</span>
        </a>
      </div>
    </article>

    <!-- Sea Isle City -->
    <article class="location-card" id="sea-isle-city">
      <div>
        <div class="location-name">Sea Isle City</div>
        <span class="location-type">Dry Cleaners</span>
      </div>

      <div class="location-address">
        <span>6216 Landis Ave.</span>
        <span>Sea Isle City, NJ 08243</span>
      </div>

      <div class="location-phone">
        <a href="tel:+16092636400">(609) 263-6400</a>
      </div>

      <div class="hours-block">
        <div class="hours-title">Store Hours</div>
        <div class="hours-list">
          <span class="hours-day">Monday</span>
          <span class="hours-time">10:00 AM – 4:00 PM</span>

          <span class="hours-day">Tuesday</span>
          <span class="hours-time closed">Closed</span>

          <span class="hours-day">Wednesday</span>
          <span class="hours-time">10:00 AM – 4:00 PM</span>

          <span class="hours-day">Thursday</span>
          <span class="hours-time closed">Closed</span>

          <span class="hours-day">Friday</span>
          <span class="hours-time">10:00 AM – 4:00 PM</span>

          <span class="hours-day">Saturday</span>
          <span class="hours-time">10:00 AM – 3:00 PM</span>

          <span class="hours-day">Sunday</span>
          <span class="hours-time closed">Closed</span>
        </div>
      </div>

      <div class="location-actions">
        <a href="https://www.google.com/maps/search/?api=1&query=6216+Landis+Ave,+Sea+Isle+City,+NJ+08243" target="_blank" rel="noopener">
          <span>📍</span><span>Directions</span>
        </a>
        <a href="tel:+16092636400">
          <span>📞</span><span>Call</span>
        </a>
      </div>
    </article>

    <!-- Wildwood -->
    <article class="location-card" id="wildwood">
      <div>
        <div class="location-name">Wildwood</div>
        <span class="location-type">Dry Cleaners</span>
        <span class="location-type">Laundromat</span>
      </div>

      <div class="location-address">
        <span>3401 New Jersey Ave. #4</span>
        <span>Wildwood, NJ 08260</span>
      </div>

      <div class="location-phone">
        <a href="tel:+16095227719">(609) 522-7719</a>
      </div>

      <div class="hours-block">
        <div class="hours-title">Dry Cleaners Hours</div>
        <div class="hours-list">
          <span class="hours-day">Monday – Wednesday</span>
          <span class="hours-time">10:00 AM – 5:00 PM</span>

          <span class="hours-day">Thursday</span>
          <span class="hours-time closed">Closed</span>

          <span class="hours-day">Friday</span>
          <span class="hours-time">10:00 AM – 5:00 PM</span>

          <span class="hours-day">Saturday</span>
          <span class="hours-time">10:00 AM – 4:00 PM</span>

          <span class="hours-day">Sunday</span>
          <span class="hours-time closed">Closed</span>
        </div>
      </div>

      <div class="hours-block">
        <div class="hours-title">Laundromat Hours</div>
        <div class="hours-list">
          <span class="hours-day">Daily</span>
          <span class="hours-time">7:00 AM – 9:00 PM</span>
        </div>
      </div>

      <div class="location-actions">
        <a href="https://www.google.com/maps/search/?api=1&query=3401+New+Jersey+Ave+%234,+Wildwood,+NJ+08260" target="_blank" rel="noopener">
          <span>📍</span><span>Directions</span>
        </a>
        <a href="tel:+16095227719">
          <span>📞</span><span>Call</span>
        </a>
      </div>
    </article>

  </div>
</section>
