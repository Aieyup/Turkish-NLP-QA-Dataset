# Turkish-NLP-QQ-Dataset (SQuAD Format)

[Türkçe](README_TR.md) | English

This dataset contains question-answer pairs about historical places and tourist attractions in Turkey, prepared in SQuAD format. The dataset includes 15.000 QA pairs in total.

## 📝 About the Dataset

This dataset has been created using Google Gemini AI, providing a comprehensive question-answer collection about Turkey's historical and tourist attractions. The dataset is specifically prepared in SQuAD (Stanford Question Answering Dataset) format for machine learning and natural language processing studies.

### 🔍 Dataset Content

The dataset contains information about structures in the following categories:
- Historical Baths (Hamams)
- Ancient Cities and Necropolises
- Domed Tombs (Kumbets) and Monuments
- Civil Architecture Examples (Mansions and Houses)
- Historical Public Buildings
- and more.

### 📊 Dataset Characteristics

- **Format**: SQuAD (Stanford Question Answering Dataset)
- **Language**: Turkish
- **Subject**: Historical places and tourist attractions in Turkey
- **Data Type**: Question-Answer pairs
- **Source**: Content generated with Google Gemini AI

## 🎯 Example Data

### Example 1: Kozlu Ancient Site (Kırıkkale)
ENGLISH Translation:
```json ENG transtalation:
{
  "context": "Located approximately 7 km from Sulakyurt District of Kırıkkale Province, accessible via dirt roads, it is an ancient city ruins with no standing structural remains...",
  "qas": [
    {
      "question": "Which period is Kozlu Ancient Site thought to belong to?",
      "answer": "Roman Period"
    },
    {
      "question": "How can one reach Kozlu Ancient Site?",
      "answer": "via dirt roads"
    }
  ]
}
```

### Example 2: Emir Ali Kumbet (Bitlis)
ENGLISH Translation:
```json
{
  "context": "Measuring 9.10X 6.05 in total external dimensions, Emir Ali Kumbet...",
  "qas": [
    {
      "question": "What is the plan shape of the kumbet?",
      "answer": "rectangular"
    },
    {
      "question": "What are the external dimensions of Emir Ali Kumbet?",
      "answer": "9.10X 6.05"
    }
  ]
}
```

### Example 3: Kazım Civciv House (Denizli)
ENGLISH Translation:
```json
{
  "context": "Located in Serinhisar District of Denizli Province, the house is two-storied, built with stone foundation and adobe in upper floors...",
  "qas": [
    {
      "question": "What materials were used in the construction of the house?",
      "answer": "stone foundation and adobe in upper floors"
    },
    {
      "question": "What is the plan type of the house?",
      "answer": "open-sofa"
    }
  ]
}
```

## 🛠️ Dataset Creation Process

The dataset was created following these steps:

1. Collection of raw data in Excel format
2. Processing content using Google Gemini AI
3. Generation of JSON outputs for every 500 records
4. Conversion of data to SQuAD format
5. Quality control and editing

## 📊 Dataset Structure

The dataset is in JSON format, with each record containing the following information:

```json
{
    "version": "v2.0",
    "data": [
        {
            "title": "context_title",
            "paragraphs": [
                {
                    "context": "Text content",
                    "qas": [
                        {
                            "question": "Question text",
                            "id": "unique_id",
                            "answers": [
                                {
                                    "text": "Answer text",
                                    "answer_start": integer
                                }
                            ]
                        }
                    ]
                }
            ]
        }
    ]
}
```

## 🎯 Use Cases

- Training Turkish Natural Language Processing models
- Developing Question-Answering systems
- Historical and cultural heritage information systems
- Tourism applications
- Educational material development

## 📦 Requirements

Libraries used to create the dataset:

- Python 3.x
- pandas
- google.generativeai
- json
- logging

## 🤝 Contributing

To contribute to the dataset:

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Submit a pull request

## 📄 License

This dataset is licensed under the GNU General Public License v3.0 (GPL-3.0). This means you are free to:
- Use the dataset for commercial purposes
- Modify the dataset
- Distribute the dataset
- Patent the dataset
- Use the dataset for private use

For more details, see the [LICENSE](LICENSE) file or visit [GNU GPL v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).

## 📞 Contact
**EN**: For project development and collaboration:
- Email: [eyup.tp@hotmail.com](mailto:eyup.tp@hotmail.com)
For questions and feedback about the dataset, please [create an issue](https://github.com/yourusername/Turkish-NLP-QQ-Dataset/issues) in this repository.
---
