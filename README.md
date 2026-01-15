Here is a professionally structured README.md file for your GitHub repository. It includes a clear project overview, data structure details, and contribution guidelines to make it a high-quality resource for the developer community.

Sri Lanka Railway Station List (JSON)
A comprehensive and structured dataset of Sri Lanka's railway network. This repository provides a complete list of all Major Stations, Sub-Stations, and Halts categorized by line, complete with their geographic coordinates (latitude and longitude).

🌟 Overview
The Sri Lankan railway network consists of approximately 1,500+ km of track spreading across 9 primary lines. For developers building travel, logistics, or navigation apps, finding a structured list that distinguishes between a major hub (like Colombo Fort) and a minor halt (like Secretariat Halt) can be difficult.

This project aims to be the "single source of truth" for SL Railway station metadata.

📂 Data Structure
The data is organized by Line to ensure logical grouping. Each station entry follows this schema:

JSON

{
  "name": "Station Name",
  "lat": 6.9344,
  "lng": 79.8501,
  "type": "Major Junction | Major | Sub-Station | Halt"
}
Station Types Explained
Major Junction: A high-traffic hub where two or more lines meet (e.g., Ragama, Polgahawela).

Major: Significant stations where most express trains stop.

Sub-Station: Smaller urban/suburban stations with permanent staff but fewer express stops.

Halt: Minor stops with minimal infrastructure, primarily for local commuters.

🛤️ Lines Included
Main Line (Colombo Fort – Badulla)

Coastal Line (Colombo Fort – Beliatta)

Northern Line (Polgahawela – Kankesanthurai)

Kelani Valley Line (Maradana – Avissawella)

Puttalam Line (Ragama – Puttalam)

Batticaloa Line (Maho Junction – Batticaloa)

Trincomalee Line (Gal Oya Junction – Trincomalee)

Mannar Line (Medawachchiya – Talaimannar)

Matale Line (Peradeniya Junction – Matale)

Mihintale Line (Anuradhapura – Mihintale)

🚀 Usage
You can fetch this data directly in your web or mobile application:

JavaScript

fetch('https://raw.githubusercontent.com/KasunPremarathna/Sri-Lanka-Railway-Station-list-/main/station_list.json')
  .then(response => response.json())
  .then(data => console.log(data));
🤝 Contributing
Contributions are welcome! If you find a missing halt or a coordinate that needs correction:

Fork the repository.

Create a new branch (git checkout -b fix-station-data).

Commit your changes.

Push to the branch and open a Pull Request.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details
