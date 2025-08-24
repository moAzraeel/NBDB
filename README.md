# NBDB

[DB root link to netlify](https://nbdb.netlify.app/id.json)

https://nbdb.netlify.app/{$file_structure}/type.json


# NBDB Folder Structure Documentation

## Root Structure
```
NBDB/
├── README.md
├── root.json (Select Level & Paths from this Json index)
└── courses/ (Combines Level & Paths with _)
    ├── course_page_data.json (Select Subjects and Chapters From this Json)
    ├── HSC_Science/
    ├── SSC_Arts/
    └── SSC_Science/
        ├── Chemistry/
        └── Physics/
            ├── Motion/
            └── Physical Quantities and Their Measurements/
                ├── chapter_index.json (Select Modules in Chapters From Here)
                ├── These Are Dummies/
                └── Introduction to Physics/                
                    ├── assets.(riv/json/gif)
                    └── module.json
```

## JSON Configuration Files

### `root.json` (Select Level and Path EG: HSC_Science)
- **Purpose**: Main navigation index for course selection
- **Contains**: Available education levels and their paths
- **Usage**: Select Level & Paths from this JSON index
- **Location**: Root directory

### `course_page_data.json` (Select Subjects: Physics, Math, Chemistry; Chapters: Motion, Vectors, etc.)
- **Purpose**: Subject and chapter organization within each course
- **Contains**: List of subjects with their chapters and icons
- **Usage**: Select Subjects and Chapters from this JSON
- **Location**: Each course directory (HSC_Science, SSC_Science, etc.)

### `chapter_index.json` (Select Modules: VectorCalculas, VectorDotCross, etc.)
- **Purpose**: Module listing and navigation within chapters
- **Contains**: Available modules and their metadata within a specific chapter
- **Usage**: Select Modules in Chapters from here
- **Location**: Each chapter directory

### `module.json` (Data of Assets: .riv files, .gif animations, .json data & the main Blog)
- **Purpose**: Individual module configuration and metadata
- **Contains**: Module-specific settings, assets, and interactive content
- **Usage**: Configure specific learning modules
- **Location**: Each module directory

## File Types and Purposes

### Configuration Files
- **`module.json`**: Module-specific configuration and metadata
- **`chapter_index.json`**: Chapter navigation and structure data
- **`course_page_data.json`**: Course-level metadata and configuration

## Content Organization Pattern

1. **Course Level**: HSC_Science, SSC_Science (education levels)
2. **Subject Level**: Biology, Chemistry, Math, Physics
3. **Chapter Level**: Motion, Vectors, Graph, Chemistry3D
4. **Module Level**: Specific topics with interactive content and quizzes

## Key Observations

- **Modular Structure**: Each learning unit has its own `module.json` for configuration
- **Quiz System**: Separate quiz modules (indicated by 'Q' suffix)
- **Asset Organization**: Visual assets are co-located with their modules
- **Scalable Design**: Structure supports easy addition of new courses, paths, and modules

This structure appears to be designed for an educational app with interactive content, supporting multiple education levels with rich multimedia


