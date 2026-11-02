AstroSage Call Center Analysis
Excel-based data analytics project analyzing call center operations for AstroSage, a Vedic astrology consultation platform. The analysis covers ~28,000 chat/call records to surface trends in revenue, guru (astrologer) performance, user behavior, and call patterns — supporting a business decision on allocating a ₹1 crore investment to improve operational efficiency, customer satisfaction, and profitability.

Overview
Tool used: Microsoft Excel — Pivot Tables, Charts, Slicers, Dashboards, Conditional Formatting, VLOOKUP, and advanced formulas (CORREL, UNIQUE, TEXT, IF/ISBLANK, etc.)
Dataset: ~28,028 records, 35 attributes (27 categorical, 8 continuous), covering chat and call consultations on the AstroSage platform (app + Gurucool website)
Outcome: A cleaned dataset, 13 objective-question analyses (each on its own sheet), a pivot-table/chart summary, and an interactive multi-page dashboard with KPI cards and trend visuals
Files
File	Description
AstroSage_analysis_KUNAL.xlsx	Main workbook — cleaned data, pivot tables, per-question analysis sheets, and dashboard
Astrosage_analysis_KUNAL.docx	Written answers to all objective questions with methodology and observations
AstroSage_KUNAL_PRAJAPATI.pptx	Presentation summarizing findings, insights, and recommendations
Data Cleaning
Inspected all 35 columns for completeness and consistency, using filters on key fields (Consultation Type, Call Status, Website, FreeCall, FreeChat)
Validated that nulls were contextually correct (e.g., Call Status is blank for Chat sessions)
Reconciled inconsistencies between Amount and NetAmount (recomputed NetAmount = Total Amount − Operation Cost)
Filled missing Region values (defaulted to "Indian") using IF/ISBLANK
Extracted Year, Month, Day, Hour from timestamps using TEXT() and Text-to-Columns
Extracted clean Guru Name using TRIM()
Pruned irrelevant columns (__v, call VR type, raw time duration, etc.)
Key Questions Answered
Table & attribute counts, data cleaning approach
Daily call volume trend and average daily volume (avg change ≈ 246 calls/day, highly volatile, no clear trend)
Monthly call volume — December highest, January lowest (January data limited to 3 days)
Total operational cost by month — December: ₹159,875.66; January: ₹8,566.43
Average calls handled per agent per day (≈1.65)
Repeat caller analysis — 3,629 total callers, 1,275 repeat callers (~35.1% of callers), contributing ~56.61% of total calls
Total sales by consultation type — Call: ₹168,442.09 (highest), Chat: ₹45,494.70, Complementary: ₹0
Call volume by User ID and Guru ID — top user made 113 calls; top guru (Guru 256) handled 1,060 calls, far above others
Correlation between call duration and customer rating — negligible (~-0.0002 to -0.007), meaning longer calls don't drive satisfaction
Highest/lowest rated gurus — Astro Pujaa Rai & Tarot Mystical top-rated (~7.5 avg); Astro Chandan lowest (~1 avg)
Average satisfaction score by month — December: 2.95, January: 2.67
Categorical vs. continuous column breakdown (27 vs. 8)
Highlights from the Dashboard & Presentation
Traffic: Gurucool website drives more traffic than the app
Revenue mix: Call consultations dominate revenue and net earnings; Complementary and Public Live Call segments contribute marginally
Call completion: Only ~41% of calls complete successfully — missed/busy/failed calls represent a major engagement gap
Peak hours: Highest call volume between 08:00–10:00
Volume spikes: Days 10–11 saw the largest surges in call volume
Satisfaction: Overall ratings are low, pointing to service quality issues
Top performer: Astro Dr. Balkrishna combines high earnings with low consultation time, suggesting strong efficiency
Recommendations
Deploy automated IVR / AI chatbot support to reduce missed/failed call rates
Scale agent availability during 08:00–10:00 peak hours and high-volume days
Balance workload distribution across gurus to reduce burnout and improve consistency
Study and replicate top-performing gurus' practices across the team
Investigate root causes of low satisfaction ratings beyond call duration
Conclusion
The analysis shows AstroSage has strong consultation volume and a loyal repeat-caller base, but faces real challenges in call completion rates, workload balance, and customer satisfaction. Addressing these — through better agent utilization, peak-hour staffing, and root-cause review of low ratings — is key to making the ₹1 crore investment pay off in efficiency and profitability.

Author: Rohit Patidar
