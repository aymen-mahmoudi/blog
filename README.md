# Aymen Mahmoudi Blog Generator

## Overview

This project is a Python-based static blog generator designed to create a structured HTML website from predefined content and menu configurations. It dynamically generates directories, HTML files, and navigation menus based on the `website_menu_contents` list in the `page_gen.py` script.

The blog generator is ideal for creating a personal blog or static website with organized categories and pages.

---

## Directory Structure

After running the script, the following directory structure will be created:

```
Blog/
├── 2D Materials/
│   ├── 2d_graphene.html
│   ├── 2d_tmds.html
│   └── 2d_charac_tech.html
├── Computer Skills/
│   ├── pc_linux.html
│   ├── pc_zotero.html
│   ├── pc_inkscape.html
│   ├── pc_latex.html
│   ├── pc_gnuplot.html
│   └── pc_gimp.html
├── Photography/
│   ├── photo_sensors.html
│   ├── photo_Lenses.html
│   ├── photo_exposure.html
│   └── photo_post-processing.html
├── Music/
│   ├── music_software.html
│   ├── music_distribution.html
│   └── mix_mas.html
├── Extra/
│   ├── extra_quotes.html
│   ├── extra_movies.html
│   ├── extra_riddles.html
│   └── extra_people.html
└── index.html
```

---

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Ensure you have Python 3.x installed on your system.

3. Place your content files in the `Update-Here` directory, organized by category.

---

## Usage

1. Run the script to generate the blog:
   ```bash
   python page_gen.py
   ```

2. The generated website will be available in the `HTML` directory.

3. Open the `index.html` file in your browser to view the blog.

---

## Customization

### Menu Structure
- Modify the `website_menu_contents` list in `page_gen.py` to change the categories and pages.

### Content
- Add or update content files in the `Update-Here` directory. Ensure the filenames match the `href` values in `website_menu_contents`.

### Styling
- Update the `Style-Sheet/jemdoc.css` file to customize the appearance of the website.

---

## Example Workflow

### Adding a New Page
1. Add a new entry to the `website_menu_contents` list in `page_gen.py`:
   ```python
   {"class": "menu-item", "href": "new_page.html", "text": "New Page"}
   ```

2. Create a corresponding content file in the `Update-Here` directory:
   ```
   Update-Here/Category/new_page.html
   ```

3. Run the script:
   ```bash
   python page_gen.py
   ```

4. The new page will be generated in the `HTML` directory.

---

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any suggestions or improvements.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Author

Aymen Mahmoudi
