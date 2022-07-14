  <!DOCTYPE html>
  <html>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.5.0/Chart.min.js"></script>
  <style>
  h1 {
  margin-top: -66px;
  margin-left:252px;
    }
  body {
    background-color: #FFFFFF;
    font-family: Arial, Helvetica, sans-serif;
    display: flex;
    min-height: 100vh;

  }
  .danhthu {
    width:  520px;
    height: 274px;
    border-radius: 10px;
    background: #FFFFFF;
    padding: 30px;
    margin-top:50px;
    margin-left:235px;
    border-style: outset;
  }
  .qwert {
    width: 1440px;
    height: 120px;
    background: #D9D9D9;
    padding:0;
    position: static;
    border: 3px;
  }
  .qwer{
    width: 1440px;
    height: 62px;
    background: #000000; 
    }
  .cotdoc{
    width: 212px;
    height: 854px;
    margin-top: -385px;
    background-color: #817F7F;
    border: 3px;
    }
  .chunhat1{
    width:  300px;
    height: 274px;
    border-radius: 10px;
    background: #ffffff;
    border-style: outset;
    margin-top: -281px;
    margin-left: 565px; 
    padding: 30px;
  }
  .chunhat2{
    width:  1205px;
    height: 274px;
    border-radius: 10px;
    background: #ffffff;
    border-style: outset;
    margin-top: -450px;
    margin-left: 235px; 
    padding: 30px;
  }
  </style>

  <body>
  <div class="qwert"><img src="New Folder/11111.png" alt="Logoautocar" width="212px" height="120px">
  <div class="qwer"><h1 style="color: white;">Ô tô &nbsp; Đánh Giá &nbsp; Văn Hóa Xe &nbsp; Kỹ Thuật và Tư Vấn &nbsp; Bảng Giá Xe</h1>
  <div class="danhthu">
  <canvas id="Danh Thu" style="width:100%;max-width:500px"></canvas>

  <script>
  var xValues = ["Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov", "Dec"];
  var yValues = [18,10,7,14,6,20,0,0,0,0,0,0,0,10];
  var barColors ="#0075FF";

  new Chart("Danh Thu", {
    type: "bar",
    data: {
      labels: xValues,
      datasets: [{
        backgroundColor: barColors,
        data: yValues
      }]
    },
    options: {
      title: {
        display: 2022,
        text: "Danh Thu"
      }
    }
  });
  </script>
  <div class="chunhat1">
    <canvas id="myChart" style="width:100%;max-width:280px"></canvas>

    <script>
    var xValues = ["Mercedes Benz", "Huyndai", "Marda", "Kia", "Honda"];
    var yValues = [8, 4, 3, 1, 2];
    var barColors = [
      "#b91d47",
      "#00aba9",
      "#2b5797",
      "#e8c3b9",
      "#1e7145"
    ];
    
    new Chart("myChart", {
      type: "doughnut",
      data: {
        labels: xValues,
        datasets: [{
          backgroundColor: barColors,
          data: yValues
        }]
      },
      options: {
        title: {
          display: true,
          text: "Xe ban thang 6"
        }
      }
    });
    </script>
  </div>
  </div>
  <div class="cotdoc"></div>
  <div class="chunhat2"></div>
  </body>
  </html>
