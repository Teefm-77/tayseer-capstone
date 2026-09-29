


# Capstone Project: Tayseer Dataset Analysis

* **Course Name:** Data Visualization and Storytelling  
* **Student Name:** TAIF MUBARAK ALSHAMMARI 
* **SDAIA Academy Link:** https://github.com/SDAIAAcademy  
* **Dataset Link:** [Tayseer Services Dataset on Google Drive](https://drive.google.com/file/d/1HIimBlNb-15QX46qg9FPy0rA5hoLlMg6/view?usp=drive_link)
  
  
**1. Audience, Decision Question & Scope**

-Target Audience: Operations & Service Delivery Director at Tayseer.

-Decision Question: Which service category requires immediate operational re-engineering due to excessive         processing times, and how is the national digital adoption trend progressing across regions?

-Scope: Aggregate monthly performance data across Saudi regions, service categories, and delivery channels from   2022 to 2026.

**2. Visual Analysis & Findings**

Chart 1: National Digital Adoption Trend (2022–2026)

Chart 2: Average Completion Time Across Service Categories

**3. Story & Recommendations**

-Finding: Service completion times vary significantly across categories.

-The Justice & Notary category recorded the highest average completion time at 37.7 minutes, followed by         Business & Licensing at 33.8 minutes.

-Evidence: While overall national digital adoption shows steady growth rising from approximately 34% in early 2022 to over 61% by mid-2026 operational processing bottlenecks persist in specific service groups like Justice & Notary.

-Recommended Action: Allocate operational support and prioritize digital workflow automation specifically for the Justice & Notary category to reduce processing delays.

-Limitation / Alternative Explanation: The dataset consists of aggregated monthly metrics rather than transaction-level timestamps. 

-Consequently, higher completion times cannot be definitively attributed solely to channel inefficiencies without granular user interaction logs.

**4. Visual Design & AI Verification**

-Chart Choice Reasoning: A line chart was selected for Chart 1 to demonstrate continuous temporal progression over multiple years. 

A bar chart with 45-degree rotated category labels was used for Chart 2 to facilitate side-by-side comparison across discrete categories with clear numeric annotations.

-AI Verification Note: To handle the repeating digital_adoption_pct values across the four channels per month/region/category, data was deduplicated using .drop_duplicates() before computing monthly averages.
This ensured that channel-level duplicate records were not summed or treated as independent observations.

**5. How to Run the Code**

-Open TayseerDashboard.ipynb in Google Colab.

-Download or access tayseer_services.csv via Google Drive and upload it to the Colab session storage.

-Execute all notebook cells sequentially to reproduce the data processing and export chart1.png and chart2.png.

