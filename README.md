# Website Archiver

This project is a Python-based **Website Archiver** that allows you to download a webpage along with its linked resources (CSS, JavaScript, images, etc.) and save them locally while maintaining the folder structure.

## Features
- Downloads and saves HTML, CSS, JS, images, and other linked resources.
- Preserves folder structure based on URL paths.
- Updates links in the downloaded HTML to reference local files.
- Saves the archived website in a specified directory.

## Installation

Before running the script or Jupyter Notebook, install the required dependencies:

```bash
pip install requests beautifulsoup4
```

## Usage

### Python Script

Run the script by executing:
```bash
python WebHTMLarchiver.py
```
Modify the `url` variable in the script to specify the website you want to archive.

### Jupyter Notebook

Alternatively, use the provided Jupyter Notebook for step-by-step execution.

1. Open `WebsiteArchiver.ipynb` in Jupyter Notebook.
2. Modify the `target_url` variable to specify the website to archive.
3. Run all cells to download and save the website locally.

## Output Structure
The archived website is stored in the `CTE_archive` directory (default). The directory contains:

```
CTE_archive/
├── index.html   # Main downloaded HTML file
├── css/         # CSS files
├── js/          # JavaScript files
├── images/      # Image assets
└── other/       # Other downloaded resources
```

## Example
Archiving a website:

```python
url = "https://www2.ed.gov/datastory/cte/index.html"
archiver = WebsiteArchiver(url)
archiver.archive_website()
```

This will save the website into the `CTE_archive` folder.

## License
This project is licensed under the MIT License.

