```markdown
# AI Diagnosis and Treatment System  

## Project Overview  
- The **AI Diagnosis and Treatment System** is an advanced application designed to support healthcare professionals by analyzing patient symptoms, medical history, and generating accurate diagnoses with tailored treatment plans. It utilizes cutting-edge AI technologies, web scraping tools, and language models to ensure reliable and precise recommendations.  

---

## Features  
- **Patient Inputs**: Users provide gender, age, symptoms, and medical history as inputs.  
- **Diagnosis Generation**: Generates preliminary diagnoses based on provided information.  
- **Treatment Recommendations**: Offers detailed treatment plans, including medications, lifestyle changes, and follow-up advice.  
- **Report Generation**: Automatically creates a downloadable Word document with diagnosis and treatment details.  
- **Web Scraping Tools**: Uses CREWAI tools to gather semantic medical data from trusted sources.  

---

## Technologies Used  
- **Programming Language**: Python  
- **Framework**: Streamlit (for user interface)  
- **AI Agents**: CREWAI for task delegation and execution  
- **Language Model**: OpenAI GPT-3.5-turbo-16k for natural language understanding  
- **Web Scraping**: CREWAI tools (`ScrapeWebsiteTool`, `SerperDevTool`)  
- **Document Generation**: Python `docx` library for creating Word documents  

---

## Prerequisites  
### Tools and Dependencies  
- **Python**: Version 3.7 or above is required.  
- **API Keys**: Create a `.env` file and include the following environment variables:  
  - `OPENAI_API_KEY`: API key for OpenAI GPT  
  - `SERPER_API_KEY`: API key for Serper  

Example `.env` file:  
```env
OPENAI_API_KEY=your_openai_api_key_here
SERPER_API_KEY=your_serper_api_key_here
```  

- **Python Libraries**: Install the dependencies listed in `requirements.txt`:  
```bash
pip install -r requirements.txt
```  

---

## Installation and Setup  
1. Clone the repository:  
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```  

2. Install the required dependencies:  
   ```bash
   pip install -r requirements.txt
   ```  

3. Run the application:  
   ```bash
   streamlit run app.py
   ```  

---

## How It Works  
### **Input Section**  
- Enter the following details:  
  - **Gender**: Choose from Male, Female, or Other  
  - **Age**: A numerical value between 0 and 120  
  - **Symptoms**: Describe the symptoms (e.g., "fever, cough, headache")  
  - **Medical History**: Provide relevant medical history (e.g., "diabetes, hypertension")  

### **Diagnosis Generation**  
- The **Medical Diagnostician** agent processes the inputs to deliver a preliminary diagnosis, highlighting potential conditions.  

### **Treatment Plan Recommendation**  
- The **Treatment Advisor** agent develops a personalized treatment plan, incorporating medical history and symptoms.  

### **Downloadable Report**  
- A detailed diagnosis and treatment plan are saved as a Word document that can be downloaded directly.  

---

## File Structure  
```plaintext
├── app.py                  # Main application script
├── .env                    # Environment variables file
├── requirements.txt        # List of dependencies
├── README.md               # Project documentation
```  

---

## Customization  
- **Modify Tasks**: Adjust task descriptions and agent goals in the `diagnose_task` and `treatment_task` definitions in `app.py`.  
- **Enhance Styling**: Update the Streamlit app's appearance by modifying the CSS in the `st.markdown()` section.  

---

## Future Enhancements  
- **Multilingual Support**: Expand the application to support multiple languages.  
- **Advanced Medical Databases**: Integrate with trusted databases for improved diagnosis accuracy.  
- **Patient Monitoring**: Add features to enable ongoing health tracking.  

---

## Acknowledgments  
- **Streamlit**: For an intuitive UI framework.  
- **CREWAI**: For task-oriented AI agents and tools.  
- **OpenAI**: For advanced language models enabling intelligent responses.  

---

## License  
This project is licensed under the MIT License.  

---

## Contact  
For feedback, questions, or collaboration opportunities, feel free to reach out:  
- **Email**: [Your Email Address]  
- **LinkedIn**: [Your LinkedIn Profile]  
```  