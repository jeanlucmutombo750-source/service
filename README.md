# service<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Administration HEC</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-dark text-white">
    <div class="container mt-4">
        <div class="d-flex justify-content-between align-items-center mb-4">
            <h2>Dashboard Administrateur</h2>
            <a href="index.html" class="btn btn-outline-light">Sortir</a>
        </div>

        <div class="row text-dark mb-4">
            <div class="col-md-6">
                <div class="card bg-info p-3"><h5>Étudiants : <span id="stat-total-etudiants">0</span></h5></div>
            </div>
            <div class="col-md-6">
                <div class="card bg-warning p-3"><h5>Total Caisse : <span id="stat-total-recettes">0 $</span></h5></div>
            </div>
        </div>

        <div class="card bg-secondary text-white p-3">
            <input type="text" id="adminSearch" class="form-control mb-3" placeholder="Filtrer..." onkeyup="filtrerDonnees()">
            <table class="table table-dark table-hover">
                <thead>
                    <tr><th>Matricule</th><th>Nom</th><th>Promo</th><th>Payé</th><th>Inscr.</th><th>Actions</th></tr>
                </thead>
                <tbody id="table-corps"></tbody>
            </table>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>
