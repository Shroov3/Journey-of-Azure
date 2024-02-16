Azure Key Vault is a cloud service for securely storing and accessing
secrets. A secret is anything that you want to tightly control access
to, such as API keys, passwords, certificates, or cryptographic keys.

**Encryption**: Azure Key Vault uses AES 256-bit encryption to protect your
secrets and keys, ensuring they remain private and safe.

![1](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/74c62119-2ea4-4562-ad20-72a725f0cbaa)

**Concept:**

![2](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/a7725f10-11be-4074-84cb-e7cba5109594)

Ref -
<https://learn.microsoft.com/en-us/azure/key-vault/general/basic-concepts>

**LAB:**

**Creation of key vault**

SKU – Standard, Premier

![Picture3](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/1567760b-302c-4b04-8922-2e6f67db880b)

Here there is different types of Permission mode

![Picture4](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/ec427215-a958-4878-b390-469204e92a49)

In networking tab we can customize the virtual network as per our need
and also use private endpoint

![Picture5](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/3cb6a263-23cc-464b-9671-938328ed4916)

Azure Keyvault

![Picture6](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/386a8b09-f83f-4b13-b648-9a0c2b5242bd)

Now let’s generate a Key

Here there is 2 key types (RSA, EC)

RSA key size (max) 4096 \[interview que\]

![Picture11](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/7c8e03ed-313a-4056-a817-ee1289710efa)

The storage capacity of an Azure Key Vault is limited by the total size
of all the secrets, certificates, and keys stored within it. The maximum
size of a single Key Vault is 25 KB (25,600 bytes) for standard vaults
and 50 KB (51,200 bytes) for premium vaults

**Creating secret – Manual**

![Picture7](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/c01d6218-09fa-4842-ac55-ecf755ef5b81)

**Creating secret – Certificate**

![Picture8](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/eb2af436-4f85-450f-a971-485b362dcf18)

**Creating certificate**

![Picture9](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/1288975b-a616-4283-8b09-5e7822c1f805)

**Networking setting**

Like storage account we have Firewall & Virtual network / Private
endpoint

![Picture10](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/1bdca8db-dc2a-484d-af0b-71a9466ca04f)
