<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Penilaian Mandiri Tim – Model GRIP</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: #f4f6f8;
      padding: 2rem;
      max-width: 800px;
      margin: auto;
      color: #333;
    }
    h1, h2 {
      color: #2c3e50;
    }
    .section {
      margin-bottom: 2rem;
    }
    label {
      font-weight: 500;
      display: block;
      margin: 1rem 0 0.25rem;
    }
    select {
      width: 100%;
      padding: 0.5rem;
      border-radius: 6px;
      border: 1px solid #ccc;
    }
    button {
      padding: 1rem;
      width: 100%;
      background-color: #3498db;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      margin-top: 2rem;
      cursor: pointer;
    }
    button:hover {
      background-color: #2980b9;
    }
    .results {
      background: #ecf0f1;
      padding: 1.5rem;
      border-radius: 8px;
      margin-top: 2rem;
    }
  </style>
</head>
<body>
  <h1>Penilaian Mandiri Tim – Model GRIP</h1>
  <form id="gripForm">

    <!-- Goals -->
    <div class="section">
      <h2>🎯 Goals (Tujuan)</h2>
      <label>1. Tim memiliki tujuan jangka pendek dan panjang yang jelas.</label>
      <select name="G1" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>

      <label>2. Setiap anggota memahami bagaimana peran mereka mendukung tujuan tim.</label>
      <select name="G2" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>
    </div>

    <!-- Roles -->
    <div class="section">
      <h2>👥 Roles (Peran)</h2>
      <label>3. Setiap anggota memiliki peran yang didefinisikan dengan jelas.</label>
      <select name="R1" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>

      <label>4. Peran didistribusikan sesuai kekuatan dan keahlian anggota.</label>
      <select name="R2" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>

      <label>5. Tidak ada kebingungan atau tumpang tindih dalam tanggung jawab.</label>
      <select name="R3" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>
    </div>

    <!-- Interpersonal -->
    <div class="section">
      <h2>💬 Interpersonal (Hubungan)</h2>
      <label>6. Kami membangun kepercayaan dan rasa hormat satu sama lain.</label>
      <select name="I1" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>

      <label>7. Kami bisa memberikan umpan balik secara terbuka dan konstruktif.</label>
      <select name="I2" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>
    </div>

    <!-- Processes -->
    <div class="section">
      <h2>⚙️ Processes (Proses)</h2>
      <label>8. Tim memiliki alur kerja yang jelas dan efisien.</label>
      <select name="P1" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>

      <label>9. Pertemuan tim berjalan terstruktur dan produktif.</label>
      <select name="P2" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>

      <label>10. Keputusan dalam tim diambil secara adil dan transparan.</label>
      <select name="P3" required>
        <option value="">Pilih jawaban</option>
        <option value="1">Sangat Tidak Setuju</option>
        <option value="2">Tidak Setuju</option>
        <option value="3">Netral</option>
        <option value="4">Setuju</option>
        <option value="5">Sangat Setuju</option>
      </select>
    </div>

    <button type="button" onclick="interpretResult()">Lihat Hasil</button>
  </form>

  <div id="resultBox" class="results" style="display:none;"></div>

  <script>
    function interpretResult() {
      const form = document.getElementById('gripForm');
      const fields = ['G1','G2','R1','R2','R3','I1','I2','P1','P2','P3'];
      let values = {}, total = 0;

      fields.forEach(name => {
        const value = parseInt(form[name].value);
        if (!value) {
          alert("Mohon jawab semua pertanyaan terlebih dahulu.");
          throw new Error("Semua bidang harus diisi");
        }
        total += value;
      });

      values.Goals = parseInt(form['G1'].value) + parseInt(form['G2'].value);
      values.Roles = parseInt(form['R1'].value) + parseInt(form['R2'].value) + parseInt(form['R3'].value);
      values.Interpersonal = parseInt(form['I1'].value) + parseInt(form['I2'].value);
      values.Processes = parseInt(form['P1'].value) + parseInt(form['P2'].value) + parseInt(form['P3'].value);

      const interpretations = {
        low: "perlu perhatian dan diskusi tim lebih lanjut.",
        mid: "cukup baik, namun masih bisa ditingkatkan.",
        high: "sudah sangat kuat dalam tim Anda."
      };

      let resultHTML = `<h3>📊 Hasil Penilaian GRIP Anda</h3>`;
      for (const [area, score] of Object.entries(values)) {
        const level = score <= 6 ? 'low' : score <= 10 ? 'mid' : 'high';
        resultHTML += `<p><strong>${area}</strong>: Skor ${score} – ${interpretations[level]}</p>`;
      }

      const maxArea = Object.entries(values).reduce((a, b) => a[1] > b[1] ? a : b)[0];
      const minArea = Object.entries(values).reduce((a, b) => a[1] < b[1] ? a : b)[0];

      resultHTML += `<p><strong>Area terkuat:</strong> ${maxArea}</p>`;
      resultHTML += `<p><strong>Area yang perlu perhatian lebih:</strong> ${minArea}</p>`;

      document.getElementById("resultBox").innerHTML = resultHTML;
      document.getElementById("resultBox").style.display = "block";
    }
  </script>
</body>
</html>
