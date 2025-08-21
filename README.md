# NBDB

[DB link to netlify](https://nbdb.netlify.app/id.json)

https://nbdb.netlify.app/ -- then file structure.

# NBDB Folder Structure Documentation
## Root Structure
```
NBDB/
├── README.md
├── root.json (Select Level & Paths from this Json index)
└── Courses/ (Combines Level & Paths with _)
    ├── course_page_data.json (Select Subjects and Chapters From this Json)
    ├── HSC_Science/
    ├── SSC_Arts/
    └── SSC_Science/
        ├── Chemistry/
        └── Physics/        
            ├── Mo/
            └── Physics/
```

## File Types and Purposes

### Configuration Files
- **`module.json`**: Module-specific configuration and metadata
- **`chapter_index.json`**: Chapter navigation and structure data
- **`course_page_data.json`**: Course-level metadata and configuration

### Interactive Content
- **`.riv`**: Rive animation files (custom interactive format)
- **`.gif`**: Animated visualizations and demonstrations
- **`.json`**: Animation data, test questions, and interactive content

### Documentation
- **`.png`**: Screenshots and visual documentation

## Content Organization Pattern

1. **Course Level**: HSC_Science, SSC_Science (education levels)
2. **Subject Level**: Biology, Chemistry, Math, Physics
3. **Chapter Level**: Motion, Vectors, Graph, Chemistry3D
4. **Module Level**: Specific topics with interactive content and quizzes

## Key Observations

- **Modular Structure**: Each learning unit has its own `module.json` for configuration
- **Interactive Focus**: Heavy use of animations (`.gif`, `.riv`) for visual learning
- **Quiz System**: Separate quiz modules (indicated by 'Q' suffix)
- **Asset Organization**: Visual assets are co-located with their modules
- **Scalable Design**: Structure supports easy addition of new courses, paths, and modules

This structure appears to be designed for an educational app with interactive physics/science content, supporting multiple education levels with rich multimedia learning materials.


