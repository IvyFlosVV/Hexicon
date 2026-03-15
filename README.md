# Hexicon

**Hexicon** is a centralized library for tracking UI code snippets and color palettes, designed to provide a tactile, visual-first workspace for rapid frontend prototyping. I chose this project because managing reusable CSS components often lacks an interactive environment that allows for real-time experimentation with background colors and lighting.

## Database Schema

The application uses a SQLite database with a primary table named `snippets` to manage design assets.

| Column | Data Type | Description |
| :--- | :--- | :--- |
| `id` | INTEGER | Primary Key (Auto-incrementing) |
| `name` | TEXT | The display name of the UI component |
| `type` | TEXT | Category of the snippet (e.g., CSS, HTML, Color) |
| `tags` | TEXT | Comma-separated labels for subsequence filtering |
| `content` | TEXT | The raw code or CSS properties of the snippet |

## CRUD Operations

Users can interact with the data through the following operations:

* **Create**: Add new snippets to the library using the "+ Add New Item" button, which opens a dedicated submission form.
* **Read**: View the full collection in the main gallery, see live statistics on the Analytics Dashboard, and render individual snippets in the Interactive Playground.
* **Update**: Modify the name, type, tags, or code content of any existing snippet via the "Edit" action.
* **Delete**: Permanently remove snippets from the database using the "Delete" button on the main dashboard.

## Technical Features

* **Subsequence Fuzzy Search**: A custom search engine that handles partial and typo-prone queries for precise resource retrieval.
* **Interactive Sandbox**: Integrated with `iro.js` to allow real-time background color manipulation while previewing components.
* **Mercury Design System**: Features 3D metallic typography and a unified "Zero-Baseline" layout for visual consistency.

## Installation & Setup

1.  **Clone the Repository**:
    ```bash
    git clone [https://github.com/IvyFlosVV/hexicon.git](https://github.com/IvyFlosVV/hexicon.git)
    cd hexicon
    ```

2.  **Environment Configuration**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```

3.  **Run the Application**:
    ```bash
    python app.py
    ```
    Access the system at `http://127.0.0.1:5000`.

## Collaborative Acknowledgement

This project was developed using an **AI-Human Collaborative Workflow**.
* **Design & Engineering**: Ivy Weng
* **Collaborative Partners**: Cursor & Gemini

---

<p align="center">
  <small>Crafted with Cursor & Gemini</small>
</p>
