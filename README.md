Main Project:
Thanks for @jesselau76
https://github.com/jesselau76/ebook-GPT-translator/issues

# ebook-GPT-translator: Enhanced Reading Experience with Customized Style and Translation

This versatile tool is crafted to elevate your reading journey by enabling the conversion of ebooks from one format to another and incorporating language translation utilizing both OpenAI API and DEEPL API. It is compatible with a diverse array of file types including PDF, DOCX, EPUB, and MOBI, and outputs the transformed content into EPUB and text files. Alongside translating text into an extensive variety of languages, this application provides you the flexibility to choose your preferred translation service and GPT model for a personalized experience.

## Key Features:

- **File Format Support**: Effortlessly convert and translate PDF, DOCX, EPUB, and MOBI documents into EPUB or text files.
- **Translation Flexibility**: Utilize either OpenAI or DEEPL APIs for translations by simply selecting the desired `translation-service` in the settings.
- **Extended Language Options**: Translate your documents into numerous languages, catering to a global audience.
- **Selectable GPT Models**: Choose from different GPT models to match your translation style and accuracy needs.
- **Graphical Elements Handling**: For EPUB files, graphical elements are smartly repositioned at the beginning of chapters to preserve the reading flow.

## Prerequisites:

Ensure you have Python 3 installed on your system along with the following packages:

- pdfminer.six
- openai
- python-deepl
- tqdm
- ebooklib
- beautifulsoup4
- python-docx
- pymobi

Install all necessary Python packages via pip with the provided `requirements.txt`:

```
pip install -r requirements.txt
```

Clone the repository using:

```
git clone https://github.com/yourusername/ebook-GPT-translator.git
```



## Configuration:


Configure your API keys and preferences in the `settings.cfg` file:

```
openai-apikey = sk-xxxxxxx # Replace 'sk-xxxxxxx' with your OpenAI API key.
deepl-apikey = yourdeeplkey # Add your DEEPL API key here.
translation-service = openai # Choose between 'openai' or 'deepl' for translation.
```
Other options in the `settings.cfg` file include:

- `prompt`: Modify the language style to suit your translation needs.
- `bilingual-output`: Enable this to get a bilingual text output.
- `langcode`: Specify the language code for the output file.
- `startpage` and `endpage`: Define the page range for translations in PDF documents.

## How to Use:

To convert and/or translate an ebook, simply pass the filename to the `text_translation.py` script as follows:

```
python text_translation.py filename
```

Here are some usage examples for different file formats:

```
python text_translation.py example.pdf
python text_translation.py example.epub
python3 text_translation.py example.docx
python text_translation.py example.txt
python text_translation.py example.mobi
```

The script will utilize the settings defined in `settings.cfg` to perform the conversion and translation operations. Additionally, you can activate bilingual output or select a specific translation service as needed.

## Conclusion:

The output will be conveniently saved as an EPUB or text file with `_translated` included in the filename, ensuring easy identification. Through its intuitive design and array of features, the ebook-GPT-translator provides an innovative solution for readers and linguists alike. Embrace a customizable translation experience and dive into your favorite texts in the style and language of your choice.

## License:

This utility is made available under the MIT License.

## Disclaimer:

This tool is intended for personal use or with content that is in the public domain. Respect copyright laws and obtain the necessary permissions before converting or translating copyrighted materials. The creators of this tool assume no liability for any misuse or copyright infringement that may occur.

For any queries or suggestions, please reach out through the issues section on GitHub.
