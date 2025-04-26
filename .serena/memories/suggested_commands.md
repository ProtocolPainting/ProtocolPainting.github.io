
# Suggested Commands for Jekyll Development

## Local Development Setup

### Jekyll Installation
```
gem install jekyll bundler
```

### Create New Jekyll Project (if starting from scratch)
```
jekyll new projectname
```

### Initialize Project with Gemfile (if not already present)
```
bundle init
```

### Add Jekyll to Gemfile
```
bundle add jekyll
```

### Install Dependencies
```
bundle install
```

## Development Commands

### Run Local Development Server
```
bundle exec jekyll serve
```

### Build Site
```
bundle exec jekyll build
```

### Run with Draft Posts
```
bundle exec jekyll serve --drafts
```

### Run with LiveReload
```
bundle exec jekyll serve --livereload
```

## Windows-Specific Commands

### List Files and Directories
```
dir
```

### Change Directory
```
cd [directory]
```

### Create Directory
```
mkdir [directory]
```

### Create Empty File
```
type nul > [filename]
```

### Copy Files
```
copy [source] [destination]
```

### Move/Rename Files
```
move [source] [destination]
```

### Delete File
```
del [file]
```

### Delete Directory
```
rmdir /s /q [directory]
```

### Search for Text in Files
```
findstr /s /i "[search term]" *.html *.md
```

## Git Commands

### Initialize Git Repository
```
git init
```

### Add Files to Staging
```
git add .
```

### Commit Changes
```
git commit -m "Commit message"
```

### Create Branch
```
git branch [branch-name]
```

### Switch Branch
```
git checkout [branch-name]
```

### Push to Remote Repository
```
git push origin [branch-name]
```

### Pull from Remote Repository
```
git pull origin [branch-name]
```
