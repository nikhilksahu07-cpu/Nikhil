
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dashboard</title>

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<style>
body {
  background: #f4f6f9;
}

.sidebar {
  width: 220px;
  height: 100vh;
  position: fixed;
  background: #111;
  color: white;
}

.sidebar a {
  display: block;
  padding: 12px;
  color: white;
  text-decoration: none;
}

.sidebar a:hover {
  background: #333;
}

.content {
  margin-left: 220px;
  padding: 20px;
}

.card-box {
  padding: 15px;
  border-radius: 10px;
  color: white;
}

.profit {
  background: #28a745;
}

.loss {
  background: #dc3545;
}

/* Mobile */
@media(max-width:768px){
  .sidebar{
    position: relative;
    width: 100%;
    height: auto;
  }
  .content{
    margin-left: 0;
  }
}
</style>
</head>

<body>

<!-- Sidebar -->
<div class="sidebar">
  <h4 class="text-center p-3">My Panel</h4>
  <a href="#">Dashboard</a>
  <a href="#">Reports</a>
  <a href="#">Users</a>
  <a href="#">Settings</a>
</div>

<!-- Content -->
<div class="content">

  <!-- Header -->
  <div class="d-flex justify-content-between align-items-center mb-4">
    <h3>Dashboard</h3>
    <div>👤 Nikhil</div>
  </div>

  <!-- Cards -->
  <div class="row mb-4">
    <div class="col-md-6">
      <div class="card-box profit">
        <h5>Total Profit</h5>
        <h3>₹12,500</h3>
      </div>
    </div>

    <div class="col-md-6">
      <div class="card-box loss">
        <h5>Total Loss</h5>
        <h3>₹5,200</h3>
      </div>
    </div>
  </div>

  <!-- Table -->
  <div class="card">
    <div class="card-body">
      <h5>Profit / Loss Report</h5>

      <table class="table table-bordered mt-3">
        <thead>
          <tr>
            <th>Date</th>
            <th>Profit</th>
            <th>Loss</th>
          </tr>
        </thead>

        <tbody>
          <tr>
            <td>01 May</td>
            <td class="text-success">₹3000</td>
            <td class="text-danger">₹1000</td>
          </tr>

          <tr>
            <td>02 May</td>
            <td class="text-success">₹4000</td>
            <td class="text-danger">₹2000</td>
          </tr>

          <tr>
            <td>03 May</td>
            <td class="text-success">₹2500</td>
            <td class="text-danger">₹1500</td>
          </tr>
        </tbody>
      </table>

    </div>
  </div>

</div>

</body>
</html>
