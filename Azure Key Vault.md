Azure Key Vault is a cloud service for securely storing and accessing
secrets. A secret is anything that you want to tightly control access
to, such as API keys, passwords, certificates, or cryptographic keys.

Encryption: Azure Key Vault uses AES 256-bit encryption to protect your
secrets and keys, ensuring they remain private and safe.

![1](https://github.com/Shroov3/Journey-of-Azure/assets/113405359/74c62119-2ea4-4562-ad20-72a725f0cbaa)

Concept:

<img src="media/image2.png" style="width:4.14931in;height:2.73889in" alt="Overview of how Azure Key Vault works" />

Ref -
<https://learn.microsoft.com/en-us/azure/key-vault/general/basic-concepts>

LAB:

Creation of key vault

SKU – Standard, Premier

<img src="media/image3.png" style="width:6.26806in;height:4.48403in" />

Here there is different types of Permission mode

<img src="media/image4.png" style="width:5.57548in;height:4.15036in" />

In networking tab we can customize the virtual network as per our need
and also use private endpoint

<img src="media/image5.png" style="width:6.26806in;height:2.88889in" />

Azure Keyvault

<img src="media/image6.png" style="width:6.26111in;height:3.19375in" />

Now let’s generate a Key

Here there is 2 key types (RSA, EC)

RSA key size (max) 4096 \[interview que\]

<img src="media/image7.png" style="width:6.25347in;height:4.23889in" />

The storage capacity of an Azure Key Vault is limited by the total size
of all the secrets, certificates, and keys stored within it. The maximum
size of a single Key Vault is 25 KB (25,600 bytes) for standard vaults
and 50 KB (51,200 bytes) for premium vaults

Creating secret – Manual

<img src="media/image8.png" style="width:6.26806in;height:2.89514in" />

Creating secret – Certificate

<img src="media/image9.png" style="width:6.26806in;height:1.80833in" />

Creating certificate

<img src="media/image8.png" style="width:6.26806in;height:2.89514in" />

Networking setting

Like storage account we have Firewall & Virtual network / Private
endpoint

<img src="media/image10.png" style="width:6.26806in;height:1.41181in" />
