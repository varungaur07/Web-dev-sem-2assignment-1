<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Smart Event Dashboard</title>
  <link rel="stylesheet" href="index.css">
</head>
<body>

  <h1 class="title">🎯 Smart Event Dashboard</h1>
 /
  <div class="container">

    <!-- Add Event Card -->
    <div class="card">
      <h2>Add New Event</h2>

      <label>Event Title</label>
      <input type="text" id="title">

      <label>Event Date</label>
      <input type="date" id="date">

      <label>Category</label>
      <select id="category">
        <option>Conference</option>
        <option>Workshop</option>
        <option>Meeting</option>
        <option>Webinar</option>
      </select>

      <label>Description</label>
      <textarea id="description"></textarea>

      <button onclick="addEvent()">Add Event</button>
    </div>

    <!-- Event List Card -->
    <div class="card">
      <h2>My Events</h2>

      <div class="actions">
        <button onclick="clearEvents()">Clear All Events</button>
        <button onclick="addSampleEvents()">Add Sample Events</button>
      </div>

      <div id="eventList" class="event-list">
        <p class="empty">No events yet. Add your first event!</p>
      </div>
    </div>

  </div>

  <!-- DOM Demo -->
  <div class="card dom-card">
    <h2>DOM Manipulation Demo</h2>
    <div id="keyOutput">Press any key...</div>
  </div>

  <script src="index.js"></script>
</body>
</html>
