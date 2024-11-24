# Key-Vault-AlwaysEncrypted
Repository for demonstrating secure data management with Azure Key Vault and Always Encrypted as part of AZ-500 preparation.

**Prerequisites:**
✅ Azure Subscription
✅ Azure SQL Database
✅ Azure Key Vault
✅ SQL Server Management Studio (SSMS)

**High-Level Steps with Explanations:**

 **1. Deploy the Base Infrastructure from an ARM Template:** I started by deploying the lab environment using an ARM template provided in the lab materials. This template automated the creation of the required Azure resources, including a Key Vault, Azure SQL Database, and a virtual network.

 **2. Configure the Key Vault Resource with a Key and a Secret:** I configured Azure Key Vault to generate and store an encryption key and a secret. The key was used to encrypt sensitive data in the Azure SQL Database, and the secret was made accessible only to authorized applications.

 **3. Configure an Azure SQL Database and a Data-Driven Application:** After the Key Vault setup, I connected the Azure SQL Database to a data-driven application. I also prepared a table with sensitive data that needed to be encrypted, ensuring that the application could securely access and manage this data.

**4. Demonstrate the Use of Azure Key Vault in Encrypting the Azure SQL Database:** Finally, I enabled Always Encrypted on the Azure SQL Database and tested the encryption by querying the database through the data-driven application. I validated that the encrypted data was only accessible to the authorized application using the key from the Key Vault.

**Reference Link(s):**
https://microsoftlearning.github.io/AZ500-AzureSecurityTechnologies/Instructions/Labs/LAB_07_KeyVaultImplementingSecureDatabysettingupAlwaysEncrypted%20(2).html
