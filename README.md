<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Anime Vault Hindi</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #e0c3fc, #8e9eab); /* Soft purple-pink gradient */
      color: #333; /* Dark grey text */
      transition: background 0.3s ease, color 0.3s ease;
    }

    header {
      background: #6a7f9d; /* Soft blue-grey */
      padding: 20px;
      text-align: center;
      color: white;
      border-bottom: 4px solid #ffc107; /* Bright yellow accent */
    }

    header h1 {
      font-size: 2.8em;
      margin: 0;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3); /* Subtle shadow effect */
    }

    .container {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
      padding: 30px 10px;
    }

    .anime-folder {
      background-color: #ffffff; /* Clean white background */
      border-radius: 12px;
      width: 280px;
      padding: 20px;
      box-shadow: 0 0 20px rgba(129, 179, 199, 0.4); /* Soft, subtle shadow */
      transition: transform 0.3s ease, box-shadow 0.3s ease, border 0.3s ease;
      margin-bottom: 20px;
      border: 2px solid rgba(129, 179, 199, 0.6); /* Soft blue outline */
    }

    .anime-folder:hover {
      transform: translateY(-5px);
      box-shadow: 0 0 30px rgba(129, 179, 199, 0.6); /* Enhanced hover shadow */
      border: 2px solid rgba(255, 193, 7, 0.7); /* Lively yellow-orange hover outline */
    }

    .anime-folder h2 {
      font-size: 1.5em;
      color: #5f6d77; /* Subtle greyish blue */
      margin: 0;
      text-align: center;
    }

    .season-list {
      margin-top: 15px;
      font-size: 1em;
      color: #6b7f90; /* Soft blue-grey */
    }

    .season-list a {
      display: block;
      margin: 10px 0;
      color: #76c7c0; /* Cool cyan link */
      text-decoration: none;
      transition: color 0.3s ease;
    }

    .season-list a:hover {
      color: #ff6f61; /* Soft red-pink hover effect */
    }

    footer {
      text-align: center;
      padding: 20px;
      font-size: 0.85em;
      background: #2f3542; /* Dark background for footer */
      color: #aab7c4; /* Light grey text */
    }

    footer a {
      color: #76c7c0; /* Cyan link color */
      text-decoration: none;
    }

    footer a:hover {
      color: #ffc107; /* Yellow hover effect for links */
    }

  </style>
</head>
<body>

<header>
  <h1>Anime Vault Hindi 📺</h1>
  <p>Free Hindi Dubbed Anime | Powered by RareToon India</p>
</header>

<div class="container" id="anime-container">
  <!-- Anime Folders will be inserted here -->
</div>

<footer>
  Created by Fans | Links from RareToon India | We don’t host any files<br>
  <a href="#">Contact Us</a> | <a href="#">Privacy Policy</a>
</footer>

<script>
  const animeData = [
    {
      name: 'Naruto Shippuden',
      seasons: [
        { season: 1, link: 'https://rareanimes.online/naruto-shippuden-season-1-hindi-download-hd/' },
        { season: 2, link: 'https://rareanimes.online/naruto-shippuden-season-2-hindi-download-hd/' },
        { season: 3, link: 'https://rareanimes.online/naruto-shippuden-season-3-hind-download-hd/' },
        { season: 4, link: 'https://rareanimes.online/naruto-shippuden-season-4-hindi-download-hd/' },
        { season: 5, link: 'https://rareanimes.online/naruto-shippuden-season-5-hindi-download-hd/' }
      ]
    },
    {
      name: 'DAN DA DAN',
      seasons: [
        { season: 1, link: 'https://rareanimes.online/dandadan-season-1-in-hindi-download-hd/' }
      ]
    },
    {
      name: 'The Dragon Prince',
      seasons: [
        { season: 1, link: 'https://rareanimes.online/the-dragon-prince-season-1-hindi-download-hd/' },
        { season: 2, link: 'https://rareanimes.online/the-dragon-prince-season-2-hindi-hd/' },
        { season: 3, link: 'https://rareanimes.online/the-dragon-prince-season-3-hindi-hd/' },
        { season: 4, link: 'https://rareanimes.online/the-dragon-prince-season-4-hindi-hd/' },
        { season: 5, link: 'https://rareanimes.online/the-dragon-prince-season-5-hindi-hd/' },
        { season: 6, link: 'https://rareanimes.online/the-dragon-prince-season-6-hindi-hd/' }
      ]
    },
    {
      name: 'My Neighbor Totoro (1988)',
      seasons: [
        { season: 'Full Movie', link: 'https://rareanimes.online/my-neighbor-totoro-1988-hindi-download-hd/' }
      ]
    },
    {
      name: 'Suzume (2022)',
      seasons: [
        { season: 'Full Movie', link: 'https://rareanimes.online/suzume-2022-hindi-downlaod-hd/' }
      ]
    },
    {
      name: 'Black Clover: Sword of the Wizard King (2023)',
      seasons: [
        { season: 'Full Movie', link: 'https://rareanimes.online/black-clover-sword-of-the-wizard-king-2023-hindi-download-hd/' }
      ]
    },
    {
      name: "Kiki’s Delivery Service (1989)",
      seasons: [
        { season: 'Full Movie', link: 'https://rareanimes.online/kikis-delivery-service-1989-hindi-download-hd/' }
      ]
    },
    {
      name: 'Weathering with You (2007)',
      seasons: [
        { season: 'Full Movie', link: 'https://rareanimes.online/weathering-with-you-2007-hindi-download-hd/' }
      ]
    },
    {
      name: 'Wolf Children (2012)',
      seasons: [
        { season: 'Full Movie', link: 'https://rareanimes.online/wolf-children-2012-hindi-download-hd/' }
      ]
    },
    {
      name: 'Evangelion: 3.0 You Can (Not) Redo (2012)',
      seasons: [
        { season: 'Full Movie', link: 'https://rareanimes.online/evangelion-3-0-you-can-not-redo-2012-hindi-download-hd/' }
      ]
    },
    {
      name: 'Evangelion: 3.0+1.0 Thrice Upon A Time (2020)',
      seasons: [
        { season: 'Full Movie', link: 'https://rareanimes.online/evangelion-3-01-0-thrice-upon-a-time-2020-hindi-download-hd/' }
      ]
    }
  ];

  function renderAnimeFolders() {
    const animeContainer = document.getElementById('anime-container');
    animeContainer.innerHTML = '';

    animeData.forEach(anime => {
      const animeFolder = document.createElement('div');
      animeFolder.classList.add('anime-folder');

      let seasonsHTML = '<div class="season-list">';
      anime.seasons.forEach(season => {
        seasonsHTML += `<a href="${season.link}" target="_blank">Season ${season.season}</a>`;
      });
      seasonsHTML += '</div>';

      animeFolder.innerHTML = `<h2>${anime.name}</h2>${seasonsHTML}`;
      animeContainer.appendChild(animeFolder);
    });
  }

  renderAnimeFolders();
</script>

</body>
</html>
