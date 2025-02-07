# SMAP Soil Moisture Data Extraction & Visualization

This Jupyter Notebook provides tools for:
- **Selecting a location interactively using an interactive map**
- **Extracting SMAP soil moisture data for the selected location**
- **Visualizing the corresponding SMAP pixel boundaries**
- **Exporting monthly mean soil moisture data as CSV**

---

## 📌 Setup Instructions

### **1️⃣ Clone the Repository**
```sh
git clone https://github.com/YOUR_USERNAME/SMAP-Extraction.git
cd SMAP-Extraction
```

### **2️⃣ Create and Activate the Conda Environment**
```sh
conda env create -f environment.yml
conda activate smap_analysis
```

### **3️⃣ Authenticate Google Earth Engine**
Before running the notebook, authenticate Google Earth Engine (GEE) by running:
```sh
earthengine authenticate
```
Follow the prompts to complete the authentication.

### **4️⃣ Run Jupyter Lab**
```sh
jupyter lab
```
Open the Jupyter Notebook file (`smap_extraction.ipynb`) and run the cells in sequence.

---

## 📌 Features
✅ Interactive map selection for a **custom point location**  
✅ **Dynamically retrieves SMAP soil moisture data**  
✅ **Vectorizes the SMAP pixel boundary** and highlights it on the map  
✅ Extracts **monthly mean soil moisture** values and saves them to `smap_monthly_data.csv`  

---

## 📌 Expected Outputs

### **Console Output**
```
Selected Location: Longitude = -122.976837, Latitude = 49.117373
Using dynamically extracted SMAP scale: 9256.0 meters
SMAP data extraction completed. File saved as smap_monthly_data.csv
```

### **Generated CSV (`smap_monthly_data.csv`)**
```
sm_surface,Year,Month,Longitude,Latitude
0.413,2014,1,-122.976837,49.117373
0.390,2014,2,-122.976837,49.117373
0.425,2014,3,-122.976837,49.117373
```

### **Map Output**
- The **SMAP soil moisture image** is displayed using a **color gradient**.
- The **selected SMAP pixel is vectorized and outlined in yellow**.
- The **map automatically zooms to the correct pixel**.

---

## 📌 Contributing
Feel free to submit pull requests if you find improvements! 🎉

---

## 📌 License
This project is licensed under the MIT License.

---

