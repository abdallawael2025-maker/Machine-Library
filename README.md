<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Printing and Finishing Machine Library</title>
    <style>
        body {
            font-family: Abadi, sans-serif;
            margin: 0;
            padding: 0;
            background: url('Screenshot 2024-12-16 144414.png') repeat center center fixed;
            background-size: cover;
        }
        header {
            background-color: white;
            color: black;
            padding: 1rem;
            text-align: center;
            position: relative;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        header img {
            position: absolute;
            left: 10px;
            top: 10px;
            height: 100px;
        }

        .level-one {
            display: flex;
            justify-content: center;
            margin: 2rem auto;
        }
        .category {
            background: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
            text-align: center;
            margin: 1rem;
            padding: 1rem;
            width: 300px;
            cursor: pointer;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        .category img {
            width: 200px;
            height: 200px;
            margin-bottom: 1rem;
        }
        .category:hover {
            background: rgba(200, 200, 200, 0.8);
        }
        .level-two {
            display: none;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 2rem;
        }
        .machine {
            background: rgba(39, 39, 39, 0.5);
            border: 2px solid #ddd;
            border-radius: 5px;
            margin: 0.5rem;
            padding: 0.5rem;
            width: 300px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .machine img {
            max-width: 200px;
            margin-bottom: 2rem;
        }
        .machine h2 {
            color: #333;
            font-size: 2rem;
            margin-bottom: 1rem;
        }
        .machine p {
            color: #555;
            margin: 0rem 0;
        }
        .machine a {
            display: grid block;
            margin-top: 0.5rem;
            padding: 0.5rem 1rem;
            color: white;
            background-color: #007bff;
            text-decoration: none;
            border-radius: 15px;
        }
        .machine a:hover {
            background-color: #0056b3;
        }
        .active {
            display: flex;
        }
    .overview {
            background: rgba(255,255,255,0.5);
            border-radius: 10px;
            margin: 2rem auto;
            padding: 1.5rem;
            max-width: 1400px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            text-align: center;
            line-height: 1.2;
        }
        .overview h2 {
            font-size: 2rem;
            margin-bottom: 1rem;
        }
        .overview p {
            color: #333;
            font-size: 1.2rem;
            margin: 0;
        }
    </style>
        <script>
        function toggleLevelTwo(categoryId) {
            const allLevels = document.querySelectorAll('.level-two');
            allLevels.forEach(level => level.classList.remove('active'));
            
            const targetLevel = document.getElementById(categoryId);
            if (targetLevel) {
                targetLevel.classList.add('active');
            }
        }
    </script>
</head>
<body>
    <header>
        <img src="Central_Bank_of_Egypt_Logo.png" alt="Company Logo">
        <h1>Printing and Finishing Machine Library</h1>
    </header>
<!-- Overview Section -->
    <div class="overview">
        <h2>Overview</h2>
        <p>Welcome to the Printing and Finishing Machine Library. This platform provides comprehensive information about various machines used in the printing, finishing, and pre-press processes. Explore detailed catalogs, training materials, and spare parts catalogs for each machine category. Start by selecting a category below to learn more about the machines available.</p>
    </div>

    <!-- First Level -->
    <div class="level-one">
        <div class="category" onclick="toggleLevelTwo('printing-machines')">
            <img src="printing.png" alt="Printing Machines Icon">
            <h2>Printing Machines</h2>
        </div>
        <div class="category" onclick="toggleLevelTwo('finishing-machines')">
            <img src="finishing.png" alt="Finishing Machines Icon">
            <h2>Finishing Machines</h2>
        </div>
        <div class="category" onclick="toggleLevelTwo('Pre Press Machines')">
            <img src="pre-press.png" alt="Pre Press Machines Icon">
            <h2>Pre Press Machines</h2>
        </div>
    </div>

    <!-- Second Level -->
    <div id="printing-machines" class="level-two">
        <!-- Add the machine blocks related to Printing Machines -->
        <div class="machine">
            <img src="machine_logo1.png" alt="SUSI Logo">
            <h2>SUSI Machine</h2>
            <p>Model: SUSI IV</p>
            <p>Manufacturer:  K&B Banknote Solutions</p>
            <a href="susi.pdf" target="_blank">Catalog</a>
            <a href="SUPER SIMULTAN IV.pdf" target="_blank">Training Document</a>
            <a href="SUSI Spare.pdf" target="_blank">Spare Parts Catalog</a>
            <a href="SUSI overview.png" target="_blank">Machine overview</a>

        </div>
    <div class="machine">
            <img src="machine_logo2.png" alt="SOI Logo">
            <h2>Super orlof Machine</h2>
            <p>Model: SOI  III</p>
            <p>Manufacturer: K&B Banknote Solutions.</p>
            <a href="soi.pdf" target="_blank">Catalog</a>
            <a href="orlof trianing complete.pdf" target="_blank">Training Document</a>
            <a href="SOI Spare.pdf" target="_blank">Spare Parts Catalog</a>
            <a href="SOI overview.png" target="_blank">Machine overview</a>
        </div>
   <div class="machine">
            <img src="NS.png" alt="NS Logo">
            <h2>NS Machine</h2>
            <p>Model: GHI789</p>
            <p>Manufacturer:  K&B Banknote Solutions.</p>
            <a href="ns.pdf" target="_blank">Catalog</a>
            <a href="training/ns.pdf" target="_blank">Training Document</a>
            <a href="NS spare.pdf" target="_blank">Spare Parts Catalog</a>
            <a href="NS overview.png" target="_blank">Machine overview</a>
        </div>
   <div class="machine">
            <img src="cnpi.png" alt="CNP Logo">
            <h2>CNP Machine</h2>
            <p>Model: SN 6490350(3-4-5-6)</p>
            <p>Manufacturer:  K&B Banknote Solutions.</p>
            <a href="cnp.pdf" target="_blank">Catalog</a>
            <a href="CNP Reprt.pdf" target="_blank">Training Document</a>
            <a href="CNP Spare.pdf" target="_blank">Spare Parts Catalog</a>
            <a href="CNP overview.png" target="_blank">Machine overview</a>
        </div>
    <div class="machine">
            <img src="OPtinota.png" alt="OH Logo">
            <h2>OH Machine</h2>
            <p>Model: SN 66200701</p>
            <p>Manufacturer:  K&B Banknote Solutions.</p>
            <a href="OH.pdf" target="_blank">Catalog</a>
            <a href="training/oh.pdf" target="_blank">Training Document</a>
            <a href="OH spare.pdf" target="_blank">Spare Parts Catalog</a>
            <a href="optinota overview.png" target="_blank">Machine overview</a>
        </div>
    </div>

    <div id="finishing-machines" class="level-two">
        <!-- Add the machine blocks related to Finishing Machines -->
        <div class="machine">
            <img src="cutlink.png" alt="CutlineX Logo">
            <h2>CutlineX Machine</h2>
            <p>Model: MNO789</p>
            <p>Manufacturer:  K&B Banknote Solutions.</p>
            <a href="catalogs/cutlinex.pdf" target="_blank">Catalog</a>
            <a href="training/cutlinex.pdf" target="_blank">Training Document</a>
            <a href="gallery/cutlinex.html" target="_blank">Spare parts Catalog</a>
            <a href="finishing overview.png" target="_blank">Machine overview</a>
        </div>
   <div class="machine">
            <img src="Cutpak.png" alt="Cutpak Logo">
            <h2>Cutpak Machine</h2>
            <p>Model: Cutpak III</p>
            <p>Manufacturer:  K&B Banknote Solutions.</p>
            <a href="cutpakwiring.pdf" target="_blank">Catalog</a>
            <a href="cutpak.pdf" target="_blank">Training Document</a>
            <a href="cutpak spare.pdf" target="_blank">Spare Parts Catalog</a>
            <a href="finishing overview.png" target="_blank">Machine overview</a>
        </div>
  <div class="machine">
            <img src="BPS.png" alt="EcoPrint Logo">
            <h2>Bps Machine</h2>
            <p>Model: ZXY567</p>
            <p>Manufacturer: G&D Solutions</p>
            <a href="catalogs/ecoprint.pdf" target="_blank">Catalog</a>
            <a href="training/ecoprint.pdf" target="_blank">Training Document</a>
            <a href="gallery/ecoprint.html" target="_blank">Spare Parts Catalog</a>
            <a href="finishing overview.png" target="_blank">Critical Adjustments</a>
        </div>

    </div>

    <div id="Pre Press Machines" class="level-two">
        <!-- Add the machine blocks related to Miscellaneous Machines -->
        <div class="machine">
            <img src="ctop.png" alt="CTOP Logo">
            <h2>CTOP Machine</h2>
            <p>Model: STU456</p>
            <p>Manufacturer:  K&B Banknote Solutions.</p>
            <a href="catalogs/ctop.pdf" target="_blank">Catalog</a>
            <a href="training/ctop.pdf" target="_blank">Training Document</a>
            <a href="gallery/ctop.html" target="_blank">Spare Parts Catalog</a>
            <a href="critical/ctop.pdf" target="_blank">Critical Adjustments</a>
        </div>
   <div class="machine">
            <img src="CTIP-photo.png" alt="CTIP Logo">
            <h2>CTIP Machine</h2>
            <p>Model: K&B Banknote Solutions</p>
            <p>Manufacturer: STU Ltd.</p>
            <a href="catalogs/ctip.pdf" target="_blank">Catalog</a>
            <a href="training/ctip.pdf" target="_blank">Training Document</a>
            <a href="gallery/ctip.html" target="_blank">Spare Parts Catalog</a>
            <a href="critical/ctip.pdf" target="_blank">Critical Adjustments</a>
        </div>
  <div class="machine">
            <img src="machine_logo10.png" alt="Aqua Save Logo">
            <h2>Plate Coat</h2>
            <p>Model:K&B Banknote Solutions</p>
            <p>Manufacturer: VWX Corp.</p>
            <a href="machine2.pdf" target="_blank">Catalog</a>
            <a href="training/aqua_save.pdf" target="_blank">Training Document</a>
            <a href="gallery/aqua_save.html" target="_blank">Spare Parts Catalog</a>
        </div>
  <div class="machine">
            <img src="machine_logo12.png" alt="SpeedMaster Logo">
            <h2>Grindining Machine</h2>
            <p>Model: LMN890</p>
            <p>Manufacturer: TUV Tech</p>
            <a href="catalogs/speedmaster.pdf" target="_blank">Catalog</a>
            <a href="training/speedmaster.pdf" target="_blank">Training Document</a>
            <a href="gallery/speedmaster.html" target="_blank">Spare Parts Catalog</a>
            <a href="critical/speedmaster.pdf" target="_blank">Overview</a>
        </div>
    </div>
</body>
</html>
