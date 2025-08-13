
### **Steps to Set Up Tomcat Server in Eclipse:**

1. **Download Tomcat:**

   * Go to [Apache Tomcat official website](https://tomcat.apache.org/download-90.cgi).
   * Download the **zip** or **tar.gz** file for your platform (Windows/Linux).

2. **Install Tomcat:**

   * Extract the downloaded file to a directory (e.g., `C:\Apache\Tomcat` on Windows).

3. **Install Eclipse IDE:**

   * If not already installed, download and install [Eclipse IDE for Java EE Developers](https://www.eclipse.org/downloads/).

4. **Configure Tomcat in Eclipse:**

   * Open **Eclipse**.
   * Go to **Window** > **Preferences**.
   * Expand **Server** > **Runtime Environments**.
   * Click **Add External Servers** > Select **Apache Tomcat v9.0** (or whichever version you're using).
   * Browse and select the **Tomcat home directory** (the directory where you installed Tomcat).

5. **Create a Dynamic Web Project:**

   * Go to **File** > **New** > **Dynamic Web Project**.
   * Provide a **Project name**.
   * Set **Target runtime** to the Tomcat server you just configured.
   * Click **Finish**.

6. **Add a Servlet to the Project:**

   * Right-click the **Java Resources** > **src** folder in your project.
   * Create a new **Servlet** under `WebContent` > `WEB-INF` > `src`.
   * Implement the `doGet()` or `doPost()` methods as needed.

7. **Add Web Deployment Descriptor (web.xml):**

   * Navigate to `WebContent` > `WEB-INF` and open/create `web.xml`.
   * Define your servlet and its mapping.

8. **Deploy and Run on Tomcat:**

   * Right-click the project in the **Project Explorer**.
   * Select **Run As** > **Run on Server**.
   * Choose **Tomcat** and click **Finish**.
   * Tomcat will start, and your servlet will be deployed.

9. **Testing the Servlet:**

   * Open your web browser and navigate to `http://localhost:8080/YourProjectName/YourServlet`.
   * Check if the servlet responds as expected.


