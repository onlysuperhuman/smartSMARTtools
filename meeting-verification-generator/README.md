# Smart SMART Meeting Generator

Create meeting attendance verification PDFs in your browser. Download [index.html](index.html) and open it directly; the PDF template and JavaScript are embedded, so the generator works offline.

## Use

Enter facilitator details, a meeting date, participant names (one per line), and verification wording. You can edit the wording before selecting **Create verification PDFs**. The optional **View blank form** button opens the embedded template. The generator creates one ZIP per meeting date, with a PDF for each participant.

## CSV format

Use a CSV with a required `full_name` header. Optional headers are `file_name`, `date`, and `dear_name`:

```csv
full_name,file_name,date,dear_name
Mike Smith,,2026-09-04,Dr. Jones
Bob Davis,Bob D,2026-09-05,
```

`file_name` overrides the default first-name-and-last-initial part of the PDF filename. `dear_name` prints “Dear [name],” on that participant’s form. Otherwise, the greeting checkbox controls whether the form says “To Whom It May Concern:” or leaves the original line blank. A row without `date` uses the meeting date entered on the page. CSVs with multiple dates produce a separate ZIP for each date; pasted names all use the one date entered on the page.

## Privacy

The tool makes no uploads and needs no account. Participant names, meeting dates, and generated PDFs are never saved in browser storage. **Remember my facilitator settings** optionally stores facilitator details, preferred wording, and custom wording blocks in that browser.

## Source and independence

The template is based on the [Zoom Meeting Attendance Verification Form from SMART Recovery Volunteer HQ](https://volunteerhq.smartrecovery.org/wp-content/uploads/2021/03/Zoom-Meeting-Attendance-Verification-Form.pdf). This project is independent and is not affiliated with, endorsed by, or sponsored by SMART Recovery.
