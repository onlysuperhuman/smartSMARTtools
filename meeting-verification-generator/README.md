# Smart SMART Meeting Generator

Create SMART Recovery meeting attendance verification PDFs for one or more participants. The tool groups PDFs by meeting date and provides a ZIP download for each date.

## Use

Open [index.html](index.html) in a browser. Enter your facilitator details, choose or edit the verification wording, then add participant names (one per line) or select a CSV with a `full_name` column. Enter a meeting date and click **Create verification PDFs**. A CSV can also include `file_name` and `date` columns; multiple dates produce separate ZIPs.

The HTML file includes its PDF template and JavaScript libraries, so it works offline. Participant names, meeting dates, and generated PDFs stay in the browser. If you select **Remember my facilitator settings**, the browser stores only your facilitator details and wording preferences on that computer.
