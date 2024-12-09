# Data Analyst

Email: henriqueegarcia2000@gmail.com  
LinkedIn: [linkedin.com/in/henrique-souza-Garcia](https://www.linkedin.com/in/henrique-souza-Garcia/)

---

## Education

- **Bachelor's degree in Statistics**  
  Federal University of Uberlândia, Uberlândia, Brazil  
  **(03/2020 - 04/2024)**

- **Master's degree in Artificial Intelligence**  
  Federal University of Uberlândia, Uberlândia, Brazil  
  **(07/2024 - 07/2027)**

## Additional Courses

- **Data Science Analytics**  
  ASN.Rocks – 76 hours
- **Introduction to Power BI** – 8 hours

---

## Professional Experience

### Mid Data Analyst at iFood  
**08/2024 - Present**  
Part of the Data Analytics team for iFood Pago, responsible for studies and analyses focused on the credit area. Main tasks include:
- Conducting studies and analysis using SQL on Databricks
- Creating and monitoring dashboards in Power BI and ThoughtSpot
- Tracking iFood's portfolio for monthly evaluation reports

### Junior Data Analyst at Tribanco  
**06/2023 - 08/2024**  
Contributed to projects using Python and SAS, with significant interaction with AWS. Main responsibilities included:
- Developing a behavior model for the business credit card
- Creating views to monitor bank policy rules and First Payment Default (FPD)
- Implementing a document validation flow with federal revenue services
- Developing a KPI dashboard for the registration area

### Data Scientist Intern at Boa Vista Serviços (Equifax)  
**02/2022 - 06/2023**  
Gained experience in statistical modeling, focusing on credit default analysis. Key tasks included:
- Developing models (LightGBM in Python) for First Payment Default and credit default
- Executing ETL processes for data creation and variable management in SQL (BigQuery)

---

## Skills

- **Programming:** Python, R, SQL, SAS
- **Data Analysis & Modeling:** Statistical Modeling, Data Analysis, Power BI, Databricks
- **Languages:** English, Portuguese
- **Tools:** GCP, Office Suite

---
## Projects
### CRM Case
<a href="https://github.com/Henriqueufu/CRM_case/blob/1e6501de6d5c03149043ef1d9fc83b3887cd5b28/Case_CRM.ipynb">
    <img src="/imagens/CRM-scaled.jpg" alt="" width="400" height="400">
</a>

[Publication](https://github.com/Henriqueufu/CRM_case/blob/1e6501de6d5c03149043ef1d9fc83b3887cd5b28/Case_CRM.ipynb)

The CRM case is a study aimed at understanding customer behaviors of a company that sells food online. The main points developed were:

- Detailed data exploration to understand the behavior of the customer base
- Creation of clusters to segment customers and enable customized actions for each group
- A predictive model designed to calculate the probability of a customer making a purchase given a marketing campaign

### Web Scraping
<a href="https://github.com/Henriqueufu/web_scraping/blob/0ef68555879a965e69931a93d2e45271b26f020c/web_scraping.ipynb">
    <img src="/imagens/web_scraping.jpg" alt="" width="500" height="300">
</a>

[Publication](https://github.com/Henriqueufu/web_scraping/blob/0ef68555879a965e69931a93d2e45271b26f020c/web_scraping.ipynb)

The web scraping technique is a powerful tool for obtaining data that is not easily available. It is important to always use this technique ethically, only consuming data for which the owners permit extraction.

### OCR
<a href="https://github.com/Henriqueufu/OCR/blob/e8cebbcd4d299d18e78befc777ee3ff9816b5f1b/OCR_Curriculo%20(1).ipynb">
    <img src="/imagens/OCR.jpeg" alt="" width="500" height="300">
</a>

[Publication](https://github.com/Henriqueufu/OCR/blob/e8cebbcd4d299d18e78befc777ee3ff9816b5f1b/OCR_Curriculo%20(1).ipynb)

OCR is another technique for obtaining data from challenging sources, in this case, images. OCR allows, for example, transforming a PDF into an image and then extracting the text from the image, which can be used as data.

---
For more details, please reach out via [LinkedIn](https://www.linkedin.com/in/henrique-souza-Garcia/) or email.



<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Previsão com LightGBM</title>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
</head>
<body>
    <h1>Previsão com LightGBM</h1>
    <form id="data-form">
        <label for="feature1">Feature 1:</label>
        <input type="number" id="feature1" name="feature1"><br><br>
        
        <label for="feature2">Feature 2:</label>
        <input type="number" id="feature2" name="feature2"><br><br>

        <!-- Adicione mais campos conforme necessário -->
        
        <button type="submit">Enviar Dados</button>
    </form>

    <h2>Resultado da Previsão</h2>
    <div id="prediction-result">A previsão aparecerá aqui.</div>

    <script>
        $('#data-form').on('submit', function(e) {
            e.preventDefault();

            // Coletar os dados do formulário
            var formData = {
                feature1: $('#feature1').val(),
                feature2: $('#feature2').val(),
                // Adicione os outros campos conforme necessário
            };

            // Enviar os dados para a API
            $.ajax({
                url: 'https://seu-servidor-api.com/predict',  // Substitua pela URL do seu servidor
                type: 'POST',
                contentType: 'application/json',
                data: JSON.stringify(formData),
                success: function(response) {
                    // Exibir o resultado
                    $('#prediction-result').text('Probabilidade: ' + response.prediction);
                },
                error: function(error) {
                    $('#prediction-result').text('Erro ao obter a previsão.');
                }
            });
        });
    </script>
</body>
</html>

