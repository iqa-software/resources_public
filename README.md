# resources_public

## LPA

### How to open a report filtered to the current record

```JavaScript
// Obtain the report ID from SQL
var report = lpa_sql("SELECT ReportID AS id FROM Report WHERE ReportName = 'Your Report Name'");

// Open the report based on the ID and filtered to the current workflow code
lpa_open('/report_viewer.aspx?id=' + report.id + '&AGIR CODE=' + lpa_wkf_code());
```
