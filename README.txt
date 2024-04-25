Indoor Navigator Requirements:
1. Install Jupyter notebook in the command prompt using command: pip install jupyter 

2. Install all required packages such as  folium, pandas, os, numpy, plugins, ipywidgets, data, json
Using PIP install command in terminal.
   PIP install json
   PIP install folium
   PIP install pandas
   PIP install os
   PIP install numpy
   PIP install plugins
   PIP install ipywidgets
   PIP install data

2. Have to change the location of the file in the code at two places.
	2.1. Open psg.ipynb notebook by running the command: jupyter notebook

        2.2. Change the Excel file location in the code:df_suburbs=pd.read_excel("C:\\Users\\sharm\\OneDrive\\Desktop\\21BIT029_RaginiV_minorProject\\RaginiV_IndoorNavigator_Project\\PSG.xlsx",sheet_name="Sheet1")

	2.3. Change the Path location in the code in vaigator class: for root, dirs, files in os.walk("C:\\Users\\sharm\\OneDrive\\Desktop\\21BIT029_RaginiV_minorProject\\RaginiV_IndoorNavigator_Project\\GeoResources"):  
            for file in files:
                self.geoResources[file.split('.')[0]] = root+'/'+file

3. Save the notebook and internet connection is necessary to fetch the map.

4. In terminal, run the command: voila psg.ipynb

5. This command will navigate us to the Indoor Navigator webpage.