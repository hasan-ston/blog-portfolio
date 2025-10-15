# Blog/Portfolio Webpage 📝

A full-stack web application that combines a personal portfolio with an interactive blog platform. Users can create, edit, and comment on blog posts while exploring a professional portfolio showcase.

## 🎯 Features

- **Blog Management**: Create, edit, and delete blog posts via admin page
- **Comment System**: Interactive commenting on blog posts
- **Portfolio Showcase**: Professional portfolio page to display projects
- **Responsive Design**: Mobile-friendly interface

## 🛠️ Tech Stack

- **Backend**: Python, Django
- **Frontend**: HTML, CSS, JavaScript
- **Database**: SQLite (default Django database)

## 📋 Prerequisites

- Python 3.x
- pip (Python package manager)

## 🚀 Installation

1. **Clone the repository**
```bash
git clone https://github.com/hasan-ston/blog-portfolio.git
```

2. **Navigate to the project directory**
```bash
cd blog-portfolio
cd rp-portfolio
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Run database migrations**
```bash
python3 manage.py migrate
```

5. **Create a superuser (optional, for admin access)**
```bash
python3 manage.py createsuperuser
```

6. **Start the development server**
```bash
python3 manage.py runserver
```

7. **Access the application**

Open your browser and visit: `http://127.0.0.1:8000/`

## 📖 Usage

### Creating Blog Posts

1. Login to your account
2. Navigate to the blog section
3. Click "Create New Post"
4. Write your content and publish

### Commenting

1. Navigate to any blog post
2. Scroll to the comments section
3. Leave your comment and submit

### Portfolio

Visit the portfolio page to view showcased projects and information

## 📁 Project Structure

```
rp-portfolio/
├── blog/                    # Blog app
├── portfolio/               # Portfolio app
├── manage.py               # Django management script
├── requirements.txt        # Python dependencies
└── ...
```

## 🚀 Future Enhancements

- [ ] Rich text editor for blog posts
- [ ] Image uploads for posts
- [ ] Social media sharing
- [ ] Search functionality
- [ ] Categories and tags for posts
- [ ] User profiles

## 👤 Author

Built as a learning project to understand Django and full-stack development.


```bash
  python3 manage.py runserver
```
