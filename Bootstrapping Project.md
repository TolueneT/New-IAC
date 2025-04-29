# Terraform setup to bootstrap a simple static website using local state files and AWS S3.

## Prerequisites

- Terraform Installed
- AWS CLI with configured credentials

## Step-by-step Implementation

1. **Initialize Terraform**
   `terraform init`
   ![alt text](<Images copy/Tinit.png>)

2. **Create the HTML files**

   - `index.html`

   ```html
   <html>
   	<body>
   		<h1>Welcome to my website, where you learn, earn and grow!</h1>
   	</body>
   </html>
   ```

   - `error.html`

   ```html
   <html>
   	<body>
   		<h1>Oops! Page not found.</h1>
   	</body>
   </html>
   ```

3. **Plan the Infrastructure**

   ```bash
   terraform plan
   ```

   ![alt text](<Images copy/Tplan.png>)

4. **Apply the Configuration**

   ```bash
   terraform apply
   ```

   ![alt text](<Images copy/Tapply.png>)

5. **Test the Output**

- The `website_url` = `"toluene-static-site-bucket-123456.s3-website-us-east-1.amazonaws.com"`

![alt text](<Images copy/final.png>)

6. **To test the error output**
   ![alt text](<Images copy/error.png>)
