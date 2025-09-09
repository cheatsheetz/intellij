# IntelliJ IDEA Cheat Sheet

## Installation and Setup

### Installation Options
```bash
# Install via JetBrains Toolbox (Recommended)
# Download from https://www.jetbrains.com/toolbox/

# Ubuntu/Debian via Snap
sudo snap install intellij-idea-community --classic

# macOS
brew install --cask intellij-idea-ce

# Windows
winget install JetBrains.IntelliJIDEA.Community
```

### First Launch Configuration
1. Import settings from previous installation or start fresh
2. Select UI theme (Darcula, Light, High Contrast)
3. Configure keymap (Default, Eclipse, Visual Studio, etc.)
4. Install required plugins
5. Set up SDK/JDK paths

## Essential Shortcuts

### General Navigation
| Shortcut | Action |
|----------|---------|
| `Ctrl+Shift+A` | Find Action |
| `Double Shift` | Search Everywhere |
| `Ctrl+N` | Go to Class |
| `Ctrl+Shift+N` | Go to File |
| `Ctrl+Alt+Shift+N` | Go to Symbol |
| `Ctrl+E` | Recent Files |
| `Ctrl+Shift+E` | Recently Edited Files |
| `Ctrl+Tab` | Switch Between Tabs |
| `Alt+1` | Project Tool Window |
| `Esc` | Focus Editor |

### Code Navigation
| Shortcut | Action |
|----------|---------|
| `Ctrl+B` | Go to Declaration |
| `Ctrl+Alt+B` | Go to Implementation |
| `Ctrl+Shift+B` | Go to Type Declaration |
| `Ctrl+U` | Go to Super Method/Class |
| `Ctrl+Alt+U` | Show UML Diagram |
| `Alt+F7` | Find Usages |
| `Ctrl+F7` | Find Usages in File |
| `Ctrl+Shift+F7` | Highlight Usages in File |
| `F2` | Next Error |
| `Shift+F2` | Previous Error |

### File Operations
| Shortcut | Action |
|----------|---------|
| `Ctrl+Alt+N` | New File/Class |
| `Ctrl+O` | Open File |
| `Ctrl+S` | Save File |
| `Ctrl+Shift+S` | Save All |
| `Ctrl+Alt+S` | Settings |
| `Ctrl+W` | Close Tab |
| `Ctrl+Shift+F4` | Close All Tabs |
| `Ctrl+F4` | Close Active Tab |

## Refactoring

### Basic Refactoring
| Shortcut | Action |
|----------|---------|
| `Shift+F6` | Rename |
| `F6` | Move |
| `F5` | Copy |
| `Ctrl+Alt+M` | Extract Method |
| `Ctrl+Alt+V` | Extract Variable |
| `Ctrl+Alt+C` | Extract Constant |
| `Ctrl+Alt+F` | Extract Field |
| `Ctrl+Alt+P` | Extract Parameter |
| `Ctrl+Alt+N` | Inline |

### Advanced Refactoring
| Shortcut | Action |
|----------|---------|
| `Ctrl+Shift+Alt+T` | Refactor This |
| `Ctrl+Alt+Shift+M` | Move Members |
| `Alt+Delete` | Safe Delete |
| `Ctrl+F6` | Change Signature |
| `Ctrl+Alt+Shift+I` | Inspect Code |
| `Ctrl+Alt+O` | Optimize Imports |
| `Ctrl+Alt+L` | Reformat Code |

### Code Generation
| Shortcut | Action |
|----------|---------|
| `Alt+Insert` | Generate Code |
| `Ctrl+O` | Override Methods |
| `Ctrl+I` | Implement Methods |
| `Alt+Shift+Insert` | Column Selection Mode |
| `Ctrl+/` | Line Comment |
| `Ctrl+Shift+/` | Block Comment |
| `Ctrl+Alt+T` | Surround With |

## Editing Features

### Selection and Multi-caret
| Shortcut | Action |
|----------|---------|
| `Ctrl+W` | Extend Selection |
| `Ctrl+Shift+W` | Shrink Selection |
| `Ctrl+D` | Duplicate Line |
| `Ctrl+Y` | Delete Line |
| `Alt+J` | Add Selection for Next Occurrence |
| `Alt+Shift+J` | Unselect Occurrence |
| `Ctrl+Alt+Shift+J` | Select All Occurrences |
| `Alt+Shift+Click` | Create Rectangular Selection |

### Code Folding
| Shortcut | Action |
|----------|---------|
| `Ctrl+NumPad+` | Expand |
| `Ctrl+NumPad-` | Collapse |
| `Ctrl+Shift+NumPad+` | Expand All |
| `Ctrl+Shift+NumPad-` | Collapse All |
| `Ctrl+.` | Fold Selection |

## Debugging

### Debug Shortcuts
| Shortcut | Action |
|----------|---------|
| `Shift+F9` | Debug |
| `Shift+F10` | Run |
| `Ctrl+F2` | Stop |
| `F9` | Resume Program |
| `F8` | Step Over |
| `F7` | Step Into |
| `Shift+F8` | Step Out |
| `Alt+F9` | Run to Cursor |
| `Ctrl+F8` | Toggle Breakpoint |
| `Ctrl+Shift+F8` | View Breakpoints |

### Debug Configuration
```xml
<!-- Example Run Configuration -->
<component name="RunManager">
  <configuration name="Application" type="Application">
    <option name="MAIN_CLASS_NAME" value="com.example.Main" />
    <option name="VM_PARAMETERS" value="-Xmx512m" />
    <option name="PROGRAM_PARAMETERS" value="--debug" />
    <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$" />
    <module name="myproject" />
  </configuration>
</component>
```

## Plugin Management

### Essential Plugins
```text
Core Development:
- Lombok
- Maven Helper
- Gradle
- SonarLint
- CheckStyle-IDEA
- SpotBugs

Version Control:
- GitToolBox
- GitHub
- .ignore

Database:
- Database Tools and SQL (bundled)
- JPA Buddy

Web Development:
- JavaScript and TypeScript
- HTML/CSS Support
- React/Vue.js plugins

Productivity:
- Key Promoter X
- CodeGlance
- Rainbow Brackets
- String Manipulation
- CamelCase
```

### Plugin Installation
1. `File → Settings → Plugins`
2. Search for plugin in Marketplace
3. Install and restart IDE
4. Configure plugin settings if needed

## Project Management

### Project Structure
```text
Project Settings (Ctrl+Alt+Shift+S):
├── Project
│   ├── Project SDK
│   ├── Project Language Level
│   └── Project Compiler Output
├── Modules
│   ├── Sources
│   ├── Dependencies
│   └── Paths
├── Libraries
└── Artifacts
```

### Build Configuration

#### Maven Configuration
```xml
<!-- pom.xml example -->
<project>
    <groupId>com.example</groupId>
    <artifactId>my-app</artifactId>
    <version>1.0.0</version>
    
    <properties>
        <maven.compiler.source>11</maven.compiler.source>
        <maven.compiler.target>11</maven.compiler.target>
    </properties>
    
    <dependencies>
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.13.2</version>
            <scope>test</scope>
        </dependency>
    </dependencies>
</project>
```

#### Gradle Configuration
```gradle
// build.gradle example
plugins {
    id 'java'
    id 'application'
}

java {
    sourceCompatibility = JavaVersion.VERSION_11
    targetCompatibility = JavaVersion.VERSION_11
}

dependencies {
    implementation 'org.springframework:spring-core:5.3.21'
    testImplementation 'junit:junit:4.13.2'
}

application {
    mainClass = 'com.example.Main'
}
```

## Code Templates and Live Templates

### Custom Live Templates
```text
Settings → Editor → Live Templates

Example Java template:
Abbreviation: sout
Template text: System.out.println($END$);
Context: Java → Statement

Example method template:
Abbreviation: pubm
Template text: 
public $RETURN_TYPE$ $METHOD_NAME$($PARAMS$) {
    $END$
}
```

### File Templates
```java
// Custom Class Template
#if (${PACKAGE_NAME} && ${PACKAGE_NAME} != "")package ${PACKAGE_NAME};#end
#parse("File Header.java")

/**
 * ${NAME}
 *
 * @author ${USER}
 * @date ${DATE}
 */
public class ${NAME} {
    
}
```

## Version Control Integration

### Git Operations
| Shortcut | Action |
|----------|---------|
| `Ctrl+K` | Commit |
| `Ctrl+Shift+K` | Push |
| `Ctrl+T` | Update Project |
| `Alt+9` | Version Control Window |
| `Ctrl+Alt+Z` | Rollback |
| `Ctrl+Shift+Alt+A` | Add to VCS |
| `Ctrl+Alt+A` | Add File to Git |

### Git Configuration
```text
Settings → Version Control → Git
- Path to Git executable
- Use credential helper
- Update method: Merge/Rebase
- Auto-update if push rejected
```

## Best Practices and Tips

### Performance Optimization
```text
Settings → Appearance & Behavior → System Settings
- Memory settings: Increase heap size
- Registry settings: Enable performance tweaks
- Disable unused plugins
- Exclude build folders from indexing
```

### Code Style Configuration
```text
Settings → Editor → Code Style
- Configure for each language
- Import/Export schemes
- EditorConfig support
- Auto-format on save
```

### Productivity Tips
1. **Use intentions and quick fixes**: `Alt+Enter`
2. **Master search everywhere**: `Double Shift`
3. **Learn refactoring shortcuts**: `Ctrl+Alt+Shift+T`
4. **Use bookmarks**: `F11` to toggle, `Shift+F11` to view
5. **Customize toolbars and menus**
6. **Use scratch files**: `Ctrl+Alt+Shift+Insert`
7. **Split editors**: Right-click tab → Split

### Code Quality
- Enable inspections for code analysis
- Use SonarLint plugin for real-time feedback
- Configure CheckStyle and SpotBugs
- Set up code coverage reporting
- Use structural search and replace

## Troubleshooting Common Issues

### Performance Issues
```bash
# Increase heap size in idea.vmoptions
-Xms2g
-Xmx4g
-XX:NewRatio=3
-XX:+UseG1GC
```

### Index Corruption
```text
1. File → Invalidate Caches and Restart
2. Delete .idea/caches folder
3. Reimport project
```

### Plugin Issues
```text
1. Disable problematic plugins
2. Safe mode: Help → Find Action → "Safe Mode"
3. Reset to default: File → Manage IDE Settings → Restore Default Settings
```

### Memory Issues
```text
1. Monitor memory usage: View → Appearance → Memory Indicator
2. Increase heap size in VM options
3. Exclude unnecessary directories from indexing
4. Close unused projects
```

## Advanced Features

### Database Tools
```sql
-- Example connection
CREATE DATABASE mydb;
USE mydb;

-- IntelliJ features:
-- Auto-completion
-- Query console
-- Data editor
-- ER diagrams
```

### Spring Framework Support
```java
// Spring Boot configuration
@SpringBootApplication
public class Application {
    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }
}

// IntelliJ provides:
// - Dependency injection assistance
// - Configuration property completion
// - Spring Boot run configurations
```

### Code Analysis Tools
```text
Analyze → Inspect Code
- Unused imports
- Code duplicates  
- Security vulnerabilities
- Performance issues
- Code style violations
```

## Customization

### Appearance Settings
```text
Settings → Appearance & Behavior → Appearance
- Theme: Darcula, Light, High Contrast
- Font size and family
- Window animations
- Tool window layout
```

### Keymap Customization
```text
Settings → Keymap
- Choose base keymap (Default, Eclipse, etc.)
- Add custom shortcuts
- Remove conflicts
- Export/Import keymaps
```

### Editor Settings
```text
Settings → Editor
- General: Auto-import, code folding
- Font: Size, line spacing, ligatures
- Color Scheme: Syntax highlighting
- Code Style: Formatting rules
- Inspections: Code analysis rules
```

## Official Documentation Links

- [IntelliJ IDEA Documentation](https://www.jetbrains.com/help/idea/)
- [Keyboard Shortcuts Reference](https://resources.jetbrains.com/storage/products/intellij-idea/docs/IntelliJIDEA_ReferenceCard.pdf)
- [Plugin Development](https://plugins.jetbrains.com/docs/intellij/)
- [Code Inspections](https://www.jetbrains.com/help/idea/code-inspection.html)
- [Debugging Guide](https://www.jetbrains.com/help/idea/debugging-code.html)
- [Version Control](https://www.jetbrains.com/help/idea/version-control-integration.html)
- [Build Tools](https://www.jetbrains.com/help/idea/gradle.html)
- [Spring Support](https://www.jetbrains.com/help/idea/spring-support.html)