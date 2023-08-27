# How-to-download-IMPAC-dataset-for-autism-detection
This Python script facilitates the download and verification of fMRI (functional magnetic resonance imaging) dataset files from the IMPAC (Imaging Modalities, Phenotypes, And Connectomes) dataset. The script is designed to simplify the process of obtaining the IMPAC fMRI dataset by automating the download, integrity check, and extraction of relevant files. The dataset is organized based on various brain atlases, such as 'basc064', 'basc122', 'basc197', 'craddock_scorr_mean', 'harvard_oxford_cort_prob_2mm', 'msdl', and 'power_2011', which represent different parcellations or divisions of the brain.
<br>
<h3>The script employs a series of functions to achieve its goal:</h3>
<ol>
  <li>It calculates the SHA-256 hash of a file to verify its integrity.</li>
  <li>It checks if the downloaded file matches the expected checksum and, if valid, extracts the contents of a ZIP archive.</li>
  <li>The '_download_fmri_data' function retrieves the dataset ZIP file associated with a chosen atlas.</li>
  <li>The '_check_integrity_atlas' function verifies if the downloaded dataset files match the expected files. If not, it triggers a re-download.</li>
  <li>The main function, 'fetch_fmri_time_series', takes user input for the desired atlas. It then checks the integrity of the dataset associated with the chosen atlas and initiates the download process if required.</li>
</ol>

<h3>To use the script: </h3>
<ol>
  <li>Ensure you have Python installed.</li>
  <li>Save the script as a '.py' file (e.g., 'download_impac_fmri.py').</li>
  <li>Open a terminal or command prompt and navigate to the script's directory.</li>
  <li>Run the script using: python 'download_impac_fmri.py'.</li>
  <li>Choose an atlas by typing its name (e.g., 'basc064', 'all', etc.).</li>
  <li>The script will display progress messages, perform the necessary downloads, integrity checks, and extraction.</li>
  <li>Once complete, the script will indicate that the download process is finished.</li>
</ol>
