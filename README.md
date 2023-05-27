# dataform-bigquery-syntax

Syntax highlighting for BigQuery flavored SQL in Dataform's .sqlx files, with support for comment tagged templates in js:

```javascript
exports.dateFromTimestamp = field => /* bq */ `
	EXTRACT(DATE FROM ${field} AT TIME ZONE 'America/Chicago')
`;
```

(Just trust me, that embedded SQL looks 👌)

### Credit

Some definitions taken from the Dataform extension: https://github.com/dataform-co/dataform/blob/main/vscode/sqlx.grammar.json

BigQuery grammar from: https://github.com/shinichi-takii/vscode-language-sql-bigquery

Comment tagged templates from: https://github.com/0x00000001A/es6-string-html

## Installing

Download: https://github.com/brianbuie/vscode-dataform-bigquery-syntax/blob/main/dataform-bigquery-syntax-0.0.1.vsix

Open your downloads folder in VScode, right click that vsix file and choose 'Install Extension VSIX'
