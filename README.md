# Enhanced ZIP Utility

A comprehensive Java-based file compression and extraction tool with advanced features and an intuitive graphical user interface.

## Features

- **File Compression & Extraction**: Standard ZIP compression and decompression capabilities
- **Advanced Compression Options**: Multiple compression levels (No Compression, Fastest, Default, Maximum)
- **Password Protection**: Basic encryption simulation for secured archives
- **Split Archives**: Divide large files into smaller parts for easier storage and transfer
- **File Filtering**: Include/exclude specific file types using patterns (e.g., *.txt, *.jpg)
- **Timestamping**: Automatically add timestamps to archive filenames
- **Integrity Verification**: Verify archive integrity after creation
- **Progress Tracking**: Real-time progress bar and status updates
- **Compression Statistics**: Detailed before/after size comparisons and compression ratios
- **Exclude Hidden Files**: Option to skip hidden system files
- **User-Friendly GUI**: Intuitive interface with tabbed options organization

## Requirements

- Java Runtime Environment (JRE) 8 or higher
- Minimum 512MB RAM (1GB recommended for large files)
- 100MB free disk space

## Installation

1. Download the latest JAR file from the releases section
2. Ensure Java is installed on your system (`java -version`)
3. Run the application using:
   ```
   java -jar EnhancedZipUtility.jar
   ```

## Usage

### Basic Compression
1. Click "Browse" next to "Source File/Folder" to select your input
2. Specify a destination path or use the auto-generated one
3. Adjust compression options as needed
4. Click "Compress" to create your ZIP archive

### Extraction
1. Select a ZIP file as the source
2. Choose a destination folder (optional)
3. Click "Extract" to decompress the archive

### Advanced Features
- **Password Protection**: Check "Encrypt with Password" and enter a password
- **Split Archives**: Enable "Split Archive" and specify part size in MB
- **File Filtering**: Enter patterns (e.g., "*.txt, *.docx") to include only specific files
- **Compression Level**: Choose between speed and compression ratio

## Building from Source

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/enhanced-zip-utility.git
   ```
2. Navigate to the project directory
3. Compile the source:
   ```
   javac EnhancedZipUtility.java
   ```
4. Run the application:
   ```
   java EnhancedZipUtility
   ```

## Technical Details

- Built using Java Swing for the graphical interface
- Utilizes java.util.zip package for compression functionality
- Implements buffered streams for efficient memory usage
- Uses Adler-32 checksum for data integrity verification
- Multi-threaded design keeps UI responsive during operations

## File Format Support

- Standard ZIP archives (.zip)
- Compatible with most common ZIP utilities

## Limitations

- Password protection is a basic simulation and not military-grade encryption
- Very large files (>4GB) may require increased memory allocation
- Split archive feature has some limitations with extremely large files

## Troubleshooting

**Application won't start:**
- Verify Java is installed correctly
- Check system meets minimum requirements

**Out of memory errors:**
- Allocate more memory: `java -Xmx1024m -jar EnhancedZipUtility.jar`

**Corrupted archives:**
- Use the verification feature after compression
- Ensure adequate disk space during operations

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For bugs or feature requests, please create an issue in the GitHub repository.

## Version History

- 1.0.0 - Initial release with basic compression/extraction
- 1.1.0 - Added advanced features (password protection, split archives, filtering)
- 1.2.0 - UI improvements and additional options

## Acknowledgments

- Built using Java Standard Edition
- Icons from [Material Design](https://material.io/resources/icons/)