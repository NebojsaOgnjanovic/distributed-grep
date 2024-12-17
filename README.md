
# **Project Features**

## **1. Large File Upload System**  
- **Resumable Uploads**:  
   - Support splitting large files into smaller chunks.  
   - Store uploaded chunks in an S3 bucket.  
   - Implement functionality to **pause** and **resume** file uploads.  

---

## **2. 100GB Text File Generator**  
- **Goal**: Generate a large, meaningful text file up to 100GB in size.  
- **Approach**:  
   - Scrape approximately **100MB** of text.  
   - Split the text into smaller, reusable chunks.  
   - Repeat the chunks until the file reaches 100GB.  
   - Optionally explore using LLMs for content generation (*budget constraints apply*).  

---

## **3. Grep Functionality**  
- **Search Capabilities**:  
   - Perform keyword-based text search.  
   - Include fuzzy search functionality for approximate matches.  
   - Return search results with surrounding context:  
     **[250 characters before] + [keyword] + [250 characters after]**.  
- **Navigation**:  
   - Provide functionality to jump to the next search result.  

---

## **4. Client Application**  
- **File Upload Form**:  
   - Interface for uploading files to the system.  
- **File List**:  
   - Display a list of uploaded files.  
- **Search Form**:  
   - Allow searching through selected files using keyword-based and fuzzy search.  
   - Display results formatted in line with the grep functionality.  
