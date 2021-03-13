---
title: Use as APIs do Microsoft Graph para configurar o logon único baseado em SAML
description: Aprenda a economizar tempo usando as APIs do Microsoft Graph para automatizar a configuração de logon único baseado em SAML.
author: kenwith
localization_priority: Priority
ms.prod: applications
ms.custom: scenarios:getting-started
ms.openlocfilehash: ea4a0a23b19b0b7a7250966f59e3a92e94a40618
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761469"
---
# <a name="configure-saml-based-single-sign-on-for-your-application-using-the-microsoft-graph-api"></a><span data-ttu-id="63743-103">Configure o logon único baseado em SAML para seu aplicativo usando a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="63743-103">Configure SAML-based single sign-on for your application using the Microsoft Graph API</span></span>

<span data-ttu-id="63743-104">Neste artigo, você aprenderá como criar e configurar um SSO (logon único) baseado em SAML para seu aplicativo no Azure AD (Azure Active Directory) usando a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="63743-104">In this article, you'll learn how to create and configure a SAML-based single sign-on (SSO) for your application in Azure Active Directory (Azure AD) using the Microsoft Graph API.</span></span> <span data-ttu-id="63743-105">A configuração do aplicativo inclui URLs básicas de SAML, uma política de mapeamento de declarações e o uso de um certificado para adicionar uma chave de assinatura personalizada.</span><span class="sxs-lookup"><span data-stu-id="63743-105">The application configuration includes basic SAML URLs, a claims mapping policy, and using a certificate to add a custom signing key.</span></span> <span data-ttu-id="63743-106">Após o aplicativo ser criado, atribua a ele um usuário como administrador.</span><span class="sxs-lookup"><span data-stu-id="63743-106">After the application is created, you assign a user to it to be an administrator.</span></span> <span data-ttu-id="63743-107">Em seguida, você pode usar uma URL para obter metadados SAML do Azure AD para configuração adicional do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63743-107">You then can use a URL to obtain Azure AD SAML metadata for additional configuration of the application.</span></span> 

<span data-ttu-id="63743-108">Este artigo usa um modelo de aplicativo Azure AD da AWS como exemplo, mas você pode usar as etapas deste artigo para qualquer aplicativo baseado em SAML na Galeria do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="63743-108">This article uses an AWS Azure AD application template as an example, but you can use the steps in this article for any SAML-based app in the Azure AD Gallery.</span></span>

>[!NOTE]
><span data-ttu-id="63743-109">As chaves e os objetos de resposta mostrados neste artigo poderiam ser reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="63743-109">The response objects and keys shown in this article might be shortened for readability.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63743-110">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63743-110">Prerequisites</span></span>

- <span data-ttu-id="63743-111">Neste tutorial, você precisa de um certificado autoassinado que o Azure AD pode usar para assinar uma resposta SAML.</span><span class="sxs-lookup"><span data-stu-id="63743-111">In this tutorial, you need a self-signed certificate that Azure AD can use to sign a SAML response.</span></span> <span data-ttu-id="63743-112">Você pode usar seu próprio certificado ou usar algo como o seguinte código C# para criar um certificado de teste:</span><span class="sxs-lookup"><span data-stu-id="63743-112">You can use your own certificate or you could use something like the following C# code to create a test certificate:</span></span>

    > <span data-ttu-id="63743-113">**Observação** Este código é **APENAS** para aprendizado e referência, e não deve ser usado como está na produção.</span><span class="sxs-lookup"><span data-stu-id="63743-113">**Note** This code is for learning and reference **ONLY** and should not be used as-is in production.</span></span>

    ```C#
    using System;
    using System.Security.Cryptography;
    using System.Security.Cryptography.X509Certificates;
    using System.Text;

    /* CONSOLE APP - PROOF OF CONCEPT CODE ONLY!!
     * This code uses a self-signed certificate and should not be used 
     * in production. This code is for reference and learning ONLY.
     */
    namespace Self_signed_cert
    {
      class Program
      {
        static void Main(string[] args)
        {
          // Generate a guid to use as a password and then create the cert.
          string password = Guid.NewGuid().ToString();
          var selfsignedCert = buildSelfSignedServerCertificate(password);

          // Print values so we can copy paste into the JSON fields.
          // Print out the private key in base64 format.
          Console.WriteLine("Private Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Pfx, password)), Environment.NewLine);

          // Print out the start date in ISO 8601 format.
          DateTime startDate = DateTime.Parse(selfsignedCert.GetEffectiveDateString()).ToUniversalTime();
          Console.WriteLine("startDateTime: " + startDate.ToString("o"));

          // Print out the end date in ISO 8601 format.
          DateTime endDate = DateTime.Parse(selfsignedCert.GetExpirationDateString()).ToUniversalTime();
          Console.WriteLine("endDateTime: " + endDate.ToString("o"));

          // Print the GUID used for keyId
          string signAndPasswordGuid = Guid.NewGuid().ToString();
          string verifyGuid = Guid.NewGuid().ToString();
          Console.WriteLine("keyId GUID for Sign and passwordCredentials: " + signAndPasswordGuid);
          Console.WriteLine("keyId GUID for Verify: " + verifyGuid);

          // Print out the password.
          Console.WriteLine("Password: {0}", password);

          // Print out a displayName to use as an example.
          Console.WriteLine("displayName: CN=Example");
          Console.WriteLine();

          // Print out the public key.
          Console.WriteLine("Public Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Cert)), Environment.NewLine);
          Console.WriteLine();

          // Generate the customKeyIdentifier using hash of thumbprint.
          Console.WriteLine("Cert thumprint: {0}{1}", selfsignedCert.Thumbprint, Environment.NewLine);
          Console.WriteLine("customKeyIdentifier:");
          string keyIdentifier = GetSha256FromThumbprint(selfsignedCert.Thumbprint);
          Console.WriteLine(keyIdentifier);
        }

        // Generate a self-signed certificate.
        private static X509Certificate2 buildSelfSignedServerCertificate(string password)
        {
          const string CertificateName = @"Microsoft Azure Federated SSO Certificate TEST";
          DateTime certificateStartDate = DateTime.UtcNow;
          DateTime certificateEndDate = certificateStartDate.AddYears(2).ToUniversalTime();

          X500DistinguishedName distinguishedName = new X500DistinguishedName($"CN={CertificateName}");

          using (RSA rsa = RSA.Create(2048))
          {
            var request = new CertificateRequest(distinguishedName, rsa, HashAlgorithmName.SHA256, RSASignaturePadding.Pkcs1);

            request.CertificateExtensions.Add (
              new X509KeyUsageExtension(X509KeyUsageFlags.DataEncipherment | X509KeyUsageFlags.KeyEncipherment | X509KeyUsageFlags.DigitalSignature, false)
            );

            var certificate = request.CreateSelfSigned(new DateTimeOffset(certificateStartDate), new DateTimeOffset(certificateEndDate));
                certificate.FriendlyName = CertificateName;

            return new X509Certificate2(certificate.Export(X509ContentType.Pfx, password), password, X509KeyStorageFlags.Exportable);
          }
        }

        // Generate hash from thumbprint.
        public static string GetSha256FromThumbprint(string thumbprint)
        {
          var message = Encoding.ASCII.GetBytes(thumbprint);
          SHA256Managed hashString = new SHA256Managed();
          return Convert.ToBase64String(hashString.ComputeHash(message));
        }
      }
    }
    ```

    <span data-ttu-id="63743-114">Para concluir este tutorial, registre os seguintes valores do seu certificado:</span><span class="sxs-lookup"><span data-stu-id="63743-114">To complete this tutorial you need to record the following values from your certificate:</span></span>

    - <span data-ttu-id="63743-115">Chave privada</span><span class="sxs-lookup"><span data-stu-id="63743-115">Private Key</span></span>
    - <span data-ttu-id="63743-116">Data e hora de início</span><span class="sxs-lookup"><span data-stu-id="63743-116">Start date and time</span></span>
    - <span data-ttu-id="63743-117">Data e hora de término</span><span class="sxs-lookup"><span data-stu-id="63743-117">End date and time</span></span>
    - <span data-ttu-id="63743-118">Senha do certificado</span><span class="sxs-lookup"><span data-stu-id="63743-118">Certificate password</span></span>
    - <span data-ttu-id="63743-119">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="63743-119">Display name</span></span>
    - <span data-ttu-id="63743-120">Chave pública</span><span class="sxs-lookup"><span data-stu-id="63743-120">Public key</span></span>
    - <span data-ttu-id="63743-121">Hash da impressão digital</span><span class="sxs-lookup"><span data-stu-id="63743-121">Hash of the thumbprint</span></span>
    - <span data-ttu-id="63743-122">Identificador de chave</span><span class="sxs-lookup"><span data-stu-id="63743-122">Key identifier</span></span>

    <span data-ttu-id="63743-123">Além dos valores do certificado, também serão necessários dois novos GUIDS para os keyIds usados.</span><span class="sxs-lookup"><span data-stu-id="63743-123">In addition to the certificate values, you also need two new GUIDS for the keyIds that are used.</span></span> <span data-ttu-id="63743-124">O exemplo a seguir mostra a saída do código listado anteriormente:</span><span class="sxs-lookup"><span data-stu-id="63743-124">The following example shows the output of the previously listed code:</span></span>

    ```
    Private Key: MIIKW...AIBAzTVKCAgfQ

    startDateTime: 2020-12-17T20:33:07.0000000Z
    endDateTime: 2022-12-17T20:33:07.0000000Z
    keyId GUID for Sign and passwordCredentials: ed4f28e8-a502-4440-bfba-6038cb8506aa
    keyId GUID for Verify: e7b8c96e-dec3-4023-9c8b-ff40fa7faa3a
    Password: 74a7e867-e4f1-49a5-82fe-2087bf53e7df
    displayName: CN=Example

    Public Key: MIIDAz...pJTZg==

    Cert thumprint: 14B73D02E5094675063DF66A42B914DAD71633D7

    customKeyIdentifier:
    dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=
    ```

- <span data-ttu-id="63743-125">Este tutorial assume que você está usando o Microsoft Graph Explorer, mas você pode usar o Postman ou criar seu próprio aplicativo cliente para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="63743-125">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="63743-126">Para chamar as APIs do Microsoft Graph neste tutorial, você precisa usar uma conta com a função de administrador global e as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="63743-126">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="63743-127">Para este tutorial, serão necessárias as permissões delegadas `Application.ReadWrite.All`, `AppRoleAssignment.ReadWrite.All`, `Policy.Read.All` e`Policy.ReadWrite.ApplicationConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="63743-127">For this tutorial, the `Application.ReadWrite.All`, `AppRoleAssignment.ReadWrite.All`, `Policy.Read.All`, and `Policy.ReadWrite.ApplicationConfiguration` delegated permissions are needed.</span></span> <span data-ttu-id="63743-128">Conclua as seguintes etapas para definir as permissões no Microsoft Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="63743-128">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>

    1. <span data-ttu-id="63743-129">Inicie o [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="63743-129">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="63743-130">Selecione **Entrar com a conta da Microsoft** e entre usando uma conta de administrador global do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="63743-130">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="63743-131">Uma vez acessado, você verá os detalhes da conta do usuário no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="63743-131">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="63743-132">Selecione o ícone de configurações à direita dos detalhes da conta do usuário e, em seguida, selecione **Selecionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="63743-132">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![Selecionar as permissões do Microsoft Graph](./images/application-saml-sso-configure-api/set-permissions.png)
        
    4. <span data-ttu-id="63743-134">Role pela lista de permissões até permissões de `AppRoleAssignment`, expanda **AppRoleAssignment (1)** e selecione a permissão **AppRoleAssignment.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="63743-134">Scroll through the list of permissions to the `AppRoleAssignment` permissions, expand **AppRoleAssignment (1)**, and select the **AppRoleAssignment.ReadWrite.All** permission.</span></span> <span data-ttu-id="63743-135">Role ainda mais para baixo pela lista de permissões de `Application`, expanda **Application (2)** e selecione a permissão **Application.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="63743-135">Scroll further down the list of permissions to the `Application` permissions, expand **Application (2)**, and select the **Application.ReadWrite.All** permission.</span></span> <span data-ttu-id="63743-136">Continue até permissões de `Policy`, expanda **Policy (13)**, e selecione as permissões **Policy.Read.All** e **Policy.ReadWrite.ApplicationConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="63743-136">Continue to the `Policy` permissions, expand **Policy (13)**, and select the **Policy.Read.All**  and **Policy.ReadWrite.ApplicationConfiguration** permissions.</span></span>

        ![Rolar e selecionar as permissões approleassignment, application e policy ](./images/application-saml-sso-configure-api/select-permissions.png)

    5. <span data-ttu-id="63743-138">Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões.</span><span class="sxs-lookup"><span data-stu-id="63743-138">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="63743-139">Você não precisa consentir em nome da organização para essas permissões.</span><span class="sxs-lookup"><span data-stu-id="63743-139">You do not need to consent on behalf of your organization for these permissions.</span></span>

        ![Aceitar o consentimento das permissões](./images/application-saml-sso-configure-api/accept-permissions.png)

## <a name="step-1-create-the-application"></a><span data-ttu-id="63743-141">Etapa 1: Criar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="63743-141">Step 1: Create the application</span></span>

<span data-ttu-id="63743-142">O Azure AD tem uma galeria que contém milhares de aplicativos pré-integrados que você pode usar como modelo para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63743-142">Azure AD has a gallery that contains thousands of pre-integrated applications that you can use as a template for your application.</span></span> <span data-ttu-id="63743-143">O modelo de aplicativo descreve os metadados para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63743-143">The application template describes the metadata for that application.</span></span> <span data-ttu-id="63743-144">Usando esse modelo, você pode criar uma instância do aplicativo e da entidade de serviço no locatário para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="63743-144">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span> 

<span data-ttu-id="63743-145">Para criar o aplicativo a partir da galeria, primeiro obtenha o identificador do modelo de aplicativo e, em seguida, use esse identificador para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63743-145">To create the application from the gallery, you first get the identifier of the application template and then use that identifier to create the application.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="63743-146">Recuperar o identificador do modelo de aplicativo da galeria</span><span class="sxs-lookup"><span data-stu-id="63743-146">Retrieve the gallery application template identifier</span></span>

 <span data-ttu-id="63743-147">Neste tutorial, recupere o identificador do modelo de aplicativo para `Amazon Web Services (AWS)`.</span><span class="sxs-lookup"><span data-stu-id="63743-147">In this tutorial, you retrieve the identifier of the application template for `Amazon Web Services (AWS)`.</span></span> <span data-ttu-id="63743-148">Registre o valor da propriedade **id** para usar posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="63743-148">Record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-149">Request</span></span>

```http
GET https://graph.microsoft.com/beta/applicationTemplates?$filter=displayName eq 'Amazon Web Services (AWS)'
```

#### <a name="response"></a><span data-ttu-id="63743-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-150">Response</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applicationTemplates",
  "value": [
    {
      "id": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
      "displayName": "Amazon Web Services (AWS)",
      "homePageUrl": "http://aws.amazon.com/",
      "supportedSingleSignOnModes": [
        "password",
        "saml",
        "external"
      ],
      "supportedProvisioningTypes": [
        "sync"
      ],
      "logoUrl": "https://az495088.vo.msecnd.net/app-logo/aws_215.png",
      "categories": [
        "developerServices",
        "topApps"
      ],
      "publisher": "Amazon",
      "description": null
    }
  ]
}
```

### <a name="create-the-application"></a><span data-ttu-id="63743-151">Criar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="63743-151">Create the application</span></span>

<span data-ttu-id="63743-152">Usando o valor **id** registrado para o modelo de aplicativo, crie uma instância do aplicativo e da entidade de serviço no locatário.</span><span class="sxs-lookup"><span data-stu-id="63743-152">Using the **id** value that you recorded for the application template, create an instance of the application and service principal in your tenant.</span></span> <span data-ttu-id="63743-153">Registre o valor da propriedade **objectId** do aplicativo e o valor da propriedade **objectId** para que a entidade de serviço possa usar posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="63743-153">Record the value of the **objectId** property of the application and the value of the **objectId** property for the service principal to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-154">Request</span></span>

```http
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```

> [!NOTE]
> <span data-ttu-id="63743-155">Aguarde algum tempo para que o aplicativo seja provisionado em seu locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="63743-155">Allow some time for the app to be provisioned into your Azure AD tenant.</span></span> <span data-ttu-id="63743-156">Não é instantâneo.</span><span class="sxs-lookup"><span data-stu-id="63743-156">It is not instant.</span></span> <span data-ttu-id="63743-157">Uma estratégia é fazer uma consulta GET sobre o objeto de aplicativo e a entidade de serviço a cada 5-10 segundos até que a consulta seja bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="63743-157">One strategy is to do a GET query on the application or service principal object every 5-10 seconds until the query is successful.</span></span>

#### <a name="response"></a><span data-ttu-id="63743-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-158">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.applicationServicePrincipal",
  "application": {
    "objectId": "8f558912-0ca3-4f1e-ab6e-66ad7fa4e7bb",
    "appId": "536c33dc-dc28-42c8-ba1d-406524d83ec3",
    "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
    "displayName": "AWS Contoso",
    "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
    "identifierUris": [],
    "publicClient": null,
    "replyUrls": [
      "https://signin.aws.amazon.com/saml"
    ],
    "logoutUrl": null,
    "samlMetadataUrl": null,
    "errorUrl": null,
    "groupMembershipClaims": null,
    "availableToOtherTenants": false
  },
  "servicePrincipal": {
    "objectId": "3161ab85-8f57-4ae0-82d3-7a1f71680b27",
    "deletionTimestamp": null,
    "accountEnabled": true,
    "appId": "536c33dc-dc28-42c8-ba1d-406524d83ec3",
    "appDisplayName": "AWS Contoso",
    "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
    "appRoleAssignmentRequired": true,
    "displayName": "AWS Contoso",
    "errorUrl": null,
    "logoutUrl": null,
    "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
    "samlMetadataUrl": null,
    "microsoftFirstParty": null,
    "publisherName": "Contoso",
    "preferredTokenSigningKeyThumbprint": null,
    "replyUrls": [
      "https://signin.aws.amazon.com/saml"
    ],
    "servicePrincipalNames": [
      "536c33dc-dc28-42c8-ba1d-406524d83ec3"
    ],
    "tags": [
      "WindowsAzureActiveDirectoryIntegratedApp"
    ],
    "notificationEmailAddresses": [],
    "keyCredentials": [],
    "passwordCredentials": []
  }
}
```

## <a name="step-2-configure-single-sign-on"></a><span data-ttu-id="63743-159">2. Configurar o logon único</span><span class="sxs-lookup"><span data-stu-id="63743-159">Step 2: Configure single sign-on</span></span>

<span data-ttu-id="63743-160">Neste tutorial, defina `saml` como modo de logon único na entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="63743-160">In this tutorial, you set `saml` as the single sign-on mode in the service principal.</span></span> <span data-ttu-id="63743-161">Use o **objectId** para a entidade de serviço gravada anteriormente.</span><span class="sxs-lookup"><span data-stu-id="63743-161">Use the **objectId** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-162">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: servicePrincipal/json

{
  "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a><span data-ttu-id="63743-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-163">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls"></a><span data-ttu-id="63743-164">Definir URLs básicas de SAML</span><span class="sxs-lookup"><span data-stu-id="63743-164">Set basic SAML URLs</span></span>

<span data-ttu-id="63743-165">Usando o **objetoId** para o aplicativo registrado anteriormente, defina o URI do identificador e redirecione o URI para a AWS no objeto de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63743-165">Using the **objectId** for the application that you recorded earlier, set the identifier URI and redirect URI for AWS in the application object.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-166">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/applications/8f558912-0ca3-4f1e-ab6e-66ad7fa4e7bb
Content-type: applications/json

{
  "web": {
    "redirectUris": [
      "https://signin.aws.amazon.com/saml"
    ] 
  },
  "identifierUris": [
    "https://signin.aws.amazon.com/saml"
  ]    
}
```

#### <a name="response"></a><span data-ttu-id="63743-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-167">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="add-app-roles-optional"></a><span data-ttu-id="63743-168">Adicionar funções de aplicativo (opcional)</span><span class="sxs-lookup"><span data-stu-id="63743-168">Add app roles (Optional)</span></span>

<span data-ttu-id="63743-169">Se o aplicativo exigir as informações da função no token, adicione a definição das funções no objeto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63743-169">If the application requires the role information in the token, add the definition of the roles in the application object.</span></span> 

> [!NOTE] 
> <span data-ttu-id="63743-170">Ao adicionar funções de aplicativo, não modifique as funções de aplicativo padrão `msiam_access`.</span><span class="sxs-lookup"><span data-stu-id="63743-170">When adding app roles, don't modify the default app roles `msiam_access`.</span></span> 

<span data-ttu-id="63743-171">Use o **objectId** para a entidade de serviço gravada anteriormente.</span><span class="sxs-lookup"><span data-stu-id="63743-171">Use the **objectId** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-172">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/serviceprincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: serviceprincipals/json

{
  "appRoles": [
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "msiam_access",
      "displayName": "msiam_access",
      "id": "7dfd756e-8c27-4472-b2b7-38c17fc5de5e",
      "isEnabled": true,
      "origin": "Application",
      "value": null
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Admin,WAAD",
      "displayName": "Admin,WAAD",
      "id": "454dc4c2-8176-498e-99df-8c4efcde41ef",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Finance,WAAD",
      "displayName": "Finance,WAAD",
      "id": "8642d5fa-18a3-4245-ab8c-a96000c1a217",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-finance,arn:aws:iam::212743507312:saml-provider/WAAD"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="63743-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-173">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a><span data-ttu-id="63743-174">3. Configurar mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="63743-174">Step 3: Configure claims mapping</span></span>

### <a name="create-a-claims-mapping-policy"></a><span data-ttu-id="63743-175">Criar uma política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="63743-175">Create a claims mapping policy</span></span>

<span data-ttu-id="63743-176">Além das declarações básicas, configure as seguintes declarações para o Azure AD emitir no token SAML:</span><span class="sxs-lookup"><span data-stu-id="63743-176">In addition to the basic claims, configure the following claims for Azure AD to emit in the SAML token:</span></span>

| <span data-ttu-id="63743-177">Nome da declaração</span><span class="sxs-lookup"><span data-stu-id="63743-177">Claim name</span></span> | <span data-ttu-id="63743-178">Origem</span><span class="sxs-lookup"><span data-stu-id="63743-178">Source</span></span>  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | <span data-ttu-id="63743-179">assignedroles</span><span class="sxs-lookup"><span data-stu-id="63743-179">assignedroles</span></span>| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | <span data-ttu-id="63743-180">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="63743-180">userprincipalname</span></span> |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | <span data-ttu-id="63743-181">"900"</span><span class="sxs-lookup"><span data-stu-id="63743-181">"900"</span></span> |
| <span data-ttu-id="63743-182">funções</span><span class="sxs-lookup"><span data-stu-id="63743-182">roles</span></span> | <span data-ttu-id="63743-183">assignedroles</span><span class="sxs-lookup"><span data-stu-id="63743-183">assignedroles</span></span> |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | <span data-ttu-id="63743-184">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="63743-184">userprincipalname</span></span> |

> [!NOTE]
> <span data-ttu-id="63743-185">Algumas chaves na política de mapeamento de declarações são sensíveis a letras maiúsculas e minúsculas (por exemplo, "Version").</span><span class="sxs-lookup"><span data-stu-id="63743-185">Some keys in the claims mapping policy are case sensitive (for example, "Version").</span></span> <span data-ttu-id="63743-186">Se você receber uma mensagem de erro como "A propriedade tem um valor inválido", isso poderia ser um problema de diferenciação de maiúsculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="63743-186">If you receive an error message such as "Property has an invalid value", it might be a case sensitive issue.</span></span>

<span data-ttu-id="63743-187">Crie a política de mapeamento de declarações e registre o valor da propriedade **id** para usar posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="63743-187">Create the claims mapping policy and record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-188">Request</span></span>

```http
POST https://graph.microsoft.com/beta/policies/claimsMappingPolicies
Content-type: claimsMappingPolicies/json

{
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

#### <a name="response"></a><span data-ttu-id="63743-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-189">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: claimsMappingPolicies/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/claimsMappingPolicies/$entity",
  "id": "218e7879-5330-4ca6-8bca-ddb1f2402e73",
  "deletedDateTime": null,
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

### <a name="assign-a-claims-mapping-policy-to-a-service-principal"></a><span data-ttu-id="63743-190">Atribuir uma política de mapeamento de declarações a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="63743-190">Assign a claims mapping policy to a service principal</span></span>

<span data-ttu-id="63743-191">Use o **objectId** para a entidade de serviço gravada anteriormente, para atribuir uma política de mapeamento de declarações a ela.</span><span class="sxs-lookup"><span data-stu-id="63743-191">Use the **objectId** for the service principal that you recorded earlier to assign a claims mapping policy to it.</span></span> <span data-ttu-id="63743-192">Use o valor da propriedade **id** para a política de mapeamento de declarações no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63743-192">Use the value of the **id** property for the claims mapping policy in the body of the request.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-193">Request</span></span>

```http
POST https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27/claimsMappingPolicies/$ref
Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73"
}
```

#### <a name="response"></a><span data-ttu-id="63743-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-194">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-4-configure-a-signing-certificate"></a><span data-ttu-id="63743-195">Etapa 4. Configurar um certificado de autenticação</span><span class="sxs-lookup"><span data-stu-id="63743-195">Step 4: Configure a signing certificate</span></span>

<span data-ttu-id="63743-196">Atribua seu certificado ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63743-196">Assign your certificate to the application.</span></span> 

#### <a name="request"></a><span data-ttu-id="63743-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-197">Request</span></span>

<span data-ttu-id="63743-198">No corpo da solicitação, forneça estes valores:</span><span class="sxs-lookup"><span data-stu-id="63743-198">In the request body, provide these values:</span></span>

<span data-ttu-id="63743-199">**keyCredentials – Assinar**</span><span class="sxs-lookup"><span data-stu-id="63743-199">**keyCredentials - Sign**</span></span>

- <span data-ttu-id="63743-200">**customKeyIdentifier** – O hash da impressão digital de certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-200">**customKeyIdentifier** - The hash of the certificate thumbprint.</span></span>
- <span data-ttu-id="63743-201">**endDateTime** – A data e hora de término do certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-201">**endDateTime** - The end date and time of the certificate.</span></span>
- <span data-ttu-id="63743-202">**keyId** – O identificador da credencial.</span><span class="sxs-lookup"><span data-stu-id="63743-202">**keyId** - The identifier for the credential.</span></span> <span data-ttu-id="63743-203">Igual à keyId para a **passwordCredentials**.</span><span class="sxs-lookup"><span data-stu-id="63743-203">Same as the keyId for the **passwordCredentials**.</span></span>
- <span data-ttu-id="63743-204">**startDateTime** – A data de início do certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-204">**startDateTime** - The start date of the certificate.</span></span>
- <span data-ttu-id="63743-205">**key** – A chave privada codificada como base 64 do certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-205">**key** - The base-64 encoded private key of the certificate.</span></span>
- <span data-ttu-id="63743-206">**displayName** – O nome de exibição das credenciais.</span><span class="sxs-lookup"><span data-stu-id="63743-206">**displayName** - The display name for the credentials.</span></span>

<span data-ttu-id="63743-207">**keyCredentials – Verificar**</span><span class="sxs-lookup"><span data-stu-id="63743-207">**keyCredentials - Verify**</span></span>

- <span data-ttu-id="63743-208">**customKeyIdentifier** – O hash da impressão digital de certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-208">**customKeyIdentifier** - The hash of the certificate thumbprint.</span></span>
- <span data-ttu-id="63743-209">**endDateTime** – A data e hora de término do certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-209">**endDateTime** - The end date and time of the certificate.</span></span>
- <span data-ttu-id="63743-210">**keyId** – O identificador da credencial.</span><span class="sxs-lookup"><span data-stu-id="63743-210">**keyId** - The identifier for the credential.</span></span>
- <span data-ttu-id="63743-211">**startDateTime** – A data de início do certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-211">**startDateTime** - The start date of the certificate.</span></span>
- <span data-ttu-id="63743-212">**key** – A chave pública codificada como base 64 do certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-212">**key** - The base-64 encoded public key of the certificate.</span></span>
- <span data-ttu-id="63743-213">**displayName** – O nome de exibição das credenciais.</span><span class="sxs-lookup"><span data-stu-id="63743-213">**displayName** - The display name for the credentials.</span></span>

<span data-ttu-id="63743-214">**passwordCredentials**</span><span class="sxs-lookup"><span data-stu-id="63743-214">**passwordCredentials**</span></span>

- <span data-ttu-id="63743-215">**customKeyIdentifier** – O hash da impressão digital de certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-215">**customKeyIdentifier** - The hash of the certificate thumbprint.</span></span>
- <span data-ttu-id="63743-216">**keyId** – O identificador da credencial.</span><span class="sxs-lookup"><span data-stu-id="63743-216">**keyId** - The identifier for the credential.</span></span> <span data-ttu-id="63743-217">Igual à keyId para a **keyCredentials – Assinar**.</span><span class="sxs-lookup"><span data-stu-id="63743-217">Same as the keyId for the **keyCredentials - Sign**.</span></span>
- <span data-ttu-id="63743-218">**endDateTime** – A data e hora de término do certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-218">**endDateTime** - The end date and time of the certificate.</span></span>
- <span data-ttu-id="63743-219">**startDateTime** – A data de início do certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-219">**startDateTime** - The start date of the certificate.</span></span>
- <span data-ttu-id="63743-220">**secretText** – A senha para o certificado.</span><span class="sxs-lookup"><span data-stu-id="63743-220">**secretText** - The password for the certificate.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: servicePrincipals/json

{
  "keyCredentials":[
    {
      "customKeyIdentifier": "dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=",
      "endDateTime": 2022-12-17T20:33:07.0000000Z",
      "keyId": "ed4f28e8-a502-4440-bfba-6038cb8506aa",
      "startDateTime": "2020-12-17T20:33:07.0000000Z",
      "type": "X509CertAndPassword",
      "usage": "Sign",
      "key":"MIIKIAIBAz.....HBgUrDgMCERE20nuTptI9MEFCh2Ih2jaaLZBZGeZBRFVNXeZmAAgIH0A==",
      "displayName": "CN=Example"
    },
    {
      "customKeyIdentifier": "dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=",
      "endDateTime": "2022-12-17T20:33:07.0000000Z",
      "keyId": "e35a7d11-fef0-49ad-9f3e-aacbe0a42c42",
      "startDateTime": "2020-12-17T20:33:07.0000000Z",
      "type": "AsymmetricX509Cert",
      "usage": "Verify",
      "key": "MIIDJzCCAg+gAw......CTxQvJ/zN3bafeesMSueR83hlCSyg==",
      "displayName": "CN=Example"
    }
  ],
  "passwordCredentials": [
    {
      "customKeyIdentifier": "dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=",
      "keyId": "ed4f28e8-a502-4440-bfba-6038cb8506aa",
      "endDateTime": "2022-01-27T19:40:33Z",
      "startDateTime": "2020-04-20T19:40:33Z",
      "secretText": "74a7e867-e4f1-49a5-82fe-2087bf53e7df"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="63743-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-221">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a><span data-ttu-id="63743-222">Adicionar a chave de assinatura personalizada</span><span class="sxs-lookup"><span data-stu-id="63743-222">Activate the custom signing key</span></span>

<span data-ttu-id="63743-223">É necessário definir a propriedade **preferredTokenSigningKeyThumbprint** da entidade de serviço para a impressão digital do certificado que você deseja que o Azure AD use para assinar a resposta SAML.</span><span class="sxs-lookup"><span data-stu-id="63743-223">You need to set the **preferredTokenSigningKeyThumbprint** property of the service principal to the thumbprint of the certificate that you want Azure AD to use to sign the SAML response.</span></span> 

#### <a name="request"></a><span data-ttu-id="63743-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-224">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27

Content-type: servicePrincipals/json

{
    "preferredTokenSigningKeyThumbprint": "14B73D02E5094675063DF66A42B914DAD71633D7"
}
```

#### <a name="response"></a><span data-ttu-id="63743-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-225">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-5-assign-users"></a><span data-ttu-id="63743-226">Etapa 5. Atribuir usuários</span><span class="sxs-lookup"><span data-stu-id="63743-226">Step 5: Assign users</span></span>

### <a name="create-a-user-account"></a><span data-ttu-id="63743-227">Criar uma conta de usuário</span><span class="sxs-lookup"><span data-stu-id="63743-227">Create a user account</span></span>

<span data-ttu-id="63743-228">Para este tutorial, crie uma conta de usuário que será adicionada ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63743-228">For this tutorial, you create a user account that is added to the application.</span></span> <span data-ttu-id="63743-229">No corpo da solicitação, altere contoso.com para o nome de domínio do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="63743-229">In the request body, change contoso.com to the domain name of your tenant.</span></span> <span data-ttu-id="63743-230">Encontre informações sobre locatários na página de visão geral do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="63743-230">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="63743-231">Registre o **id** do usuário a ser usado posteriormente neste tutorial.</span><span class="sxs-lookup"><span data-stu-id="63743-231">Record the **id** of the user to be used later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-232">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a><span data-ttu-id="63743-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-233">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "mytestuser1@contoso.com"
}
```

### <a name="assign-a-user-to-the-application"></a><span data-ttu-id="63743-234">Atribuir um usuário ao aplicativo</span><span class="sxs-lookup"><span data-stu-id="63743-234">Assign a user to the application</span></span>

<span data-ttu-id="63743-235">Atribua o usuário que você criou à entidade de serviço e atribua a função de aplicativo `Admin,WAAD`.</span><span class="sxs-lookup"><span data-stu-id="63743-235">Assign the user that you created to the service principal and assign the `Admin,WAAD` app role.</span></span> 

<span data-ttu-id="63743-236">No corpo da solicitação, forneça estes valores:</span><span class="sxs-lookup"><span data-stu-id="63743-236">In the request body, provide these values:</span></span>

- <span data-ttu-id="63743-237">**principalId** – O **id** da conta de usuário que você criou.</span><span class="sxs-lookup"><span data-stu-id="63743-237">**principalId** - The **id** of the user account that you created.</span></span>
- <span data-ttu-id="63743-238">**appRoleId** – O **id** da função de apĺicativo `Admin,WAAD` que você adicionou.</span><span class="sxs-lookup"><span data-stu-id="63743-238">**appRoleId** - The **id** of the `Admin,WAAD` app role that you added.</span></span>
- <span data-ttu-id="63743-239">**resourceId** – A **id** da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="63743-239">**resourceId** - The **id** of the service principal.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-240">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27/appRoleAssignments
Content-type: appRoleAssignments/json

{
  "principalId": "3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4",
  "principalType": "User",
  "appRoleId":"454dc4c2-8176-498e-99df-8c4efcde41ef",
  "resourceId":"3161ab85-8f57-4ae0-82d3-7a1f71680b27"
}
```

#### <a name="response"></a><span data-ttu-id="63743-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-241">Response</span></span>

```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('39406665-d521-40b7-9218-55070cae56b5')/appRoleAssignments/$entity",
  "id": "jKL4BeO2yUag4xULULSkza2HXRq_atpHrViBM89X55s",
  "deletedDateTime": null,
  "appRoleId": "454dc4c2-8176-498e-99df-8c4efcde41ef",
  "createdDateTime": "2021-02-11T22:51:36.8978032Z",
  "principalDisplayName": "MyTestUser1",
  "principalId": "05f8a28c-b6e3-46c9-a0e3-150b50b4a4cd",
  "principalType": "User",
  "resourceDisplayName": "AWS Contoso",
  "resourceId": "39406665-d521-40b7-9218-55070cae56b5"
}
```

## <a name="step-6-get-azure-ad-saml-metadata"></a><span data-ttu-id="63743-242">Etapa 6: Obter metadados SAML do Azure AD</span><span class="sxs-lookup"><span data-stu-id="63743-242">Step 6: Get Azure AD SAML metadata</span></span>

<span data-ttu-id="63743-243">Use a URL a seguir para obter os metadados do SAML do Azure AD para o aplicativo específico configurado.</span><span class="sxs-lookup"><span data-stu-id="63743-243">Use the following URL to get the Azure AD SAML metadata for the specific configured application.</span></span> <span data-ttu-id="63743-244">Os metadados contêm informações como o certificado de assinatura, o Azure AD entityID e o Azure AD SingleSignOnService, entre outras.</span><span class="sxs-lookup"><span data-stu-id="63743-244">The metadata contains information such as the signing certificate, Azure AD entityID, and Azure AD SingleSignOnService, among others.</span></span>

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

<span data-ttu-id="63743-245">A seguir, é possível ver um exemplo do que você pode ver no aplicativo:</span><span class="sxs-lookup"><span data-stu-id="63743-245">The following shows an example of what you might see for your application:</span></span>

```
<EntityDescriptor xmlns="urn:oasis:names:tc:SAML:2.0:metadata" ID="_05fbbf53-e892-43c9-9300-1f6738ace02c" entityID="https://sts.windows.net/2f82f566-5953-43f4-9251-79c6009bdf24/">
<Signature xmlns="http://www.w3.org/2000/09/xmldsig#">

...

<SingleLogoutService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
</IDPSSODescriptor>
</EntityDescriptor>
```

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="63743-246">Etapa 7: Limpar recursos</span><span class="sxs-lookup"><span data-stu-id="63743-246">Step 7: Clean up resources</span></span>

<span data-ttu-id="63743-247">Nessa etapa, remova os recursos que criou.</span><span class="sxs-lookup"><span data-stu-id="63743-247">In this step, you remove the resources that you created.</span></span>


### <a name="delete-the-application"></a><span data-ttu-id="63743-248">Excluir o aplicativo</span><span class="sxs-lookup"><span data-stu-id="63743-248">Delete the application</span></span>

<span data-ttu-id="63743-249">Exclua o aplicativo que você criou.</span><span class="sxs-lookup"><span data-stu-id="63743-249">Delete the application that you created.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-250">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-250">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/applications/4b01f51f-079b-4634-b767-7e19ad502cdb
```

#### <a name="response"></a><span data-ttu-id="63743-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-251">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-user-account"></a><span data-ttu-id="63743-252">Excluir a conta de usuário</span><span class="sxs-lookup"><span data-stu-id="63743-252">Delete the user account</span></span>

<span data-ttu-id="63743-253">Exclua a conta de usuário MyTestUser1.</span><span class="sxs-lookup"><span data-stu-id="63743-253">Delete the MyTestUser1 user account.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-254">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-254">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4
```

#### <a name="response"></a><span data-ttu-id="63743-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-255">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-claims-mapping-policy"></a><span data-ttu-id="63743-256">Excluir a política de mapeamento de declarações</span><span class="sxs-lookup"><span data-stu-id="63743-256">Delete the claims mapping policy</span></span>

<span data-ttu-id="63743-257">Exclua a política de mapeamento de declarações.</span><span class="sxs-lookup"><span data-stu-id="63743-257">Delete the claims mapping policy.</span></span>

#### <a name="request"></a><span data-ttu-id="63743-258">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63743-258">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73
```

#### <a name="response"></a><span data-ttu-id="63743-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="63743-259">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="63743-260">Confira também</span><span class="sxs-lookup"><span data-stu-id="63743-260">See also</span></span>

- <span data-ttu-id="63743-261">No AWS, você pode [habilitar o provisionamento de usuário](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api) para buscar todas as funções dessa conta do AWS.</span><span class="sxs-lookup"><span data-stu-id="63743-261">For AWS, you can [enable user provisioning](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api) to fetch all the roles from that AWS account.</span></span> <span data-ttu-id="63743-262">Para saber mais, confira [Configurar a declaração de função emitida no token SAML](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span><span class="sxs-lookup"><span data-stu-id="63743-262">For more information, see [Configure the role claim issued in the SAML token](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span></span>
- <span data-ttu-id="63743-263">[Personalizar as declarações emitidas em tokens para um aplicativo específico em um locatário](/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="63743-263">[Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
- <span data-ttu-id="63743-264">Você pode usar a API applicationTemplate para criar uma instância [Aplicativos inexistentes na galeria](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal).</span><span class="sxs-lookup"><span data-stu-id="63743-264">You can use the applicationTemplate API to instantiate [Non-Gallery apps](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal).</span></span> <span data-ttu-id="63743-265">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span><span class="sxs-lookup"><span data-stu-id="63743-265">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>
- [<span data-ttu-id="63743-266">New-SelfSignedCertificate</span><span class="sxs-lookup"><span data-stu-id="63743-266">New-SelfSignedCertificate</span></span>](/powershell/module/pkiclient/new-selfsignedcertificate?view=win10-ps)
- [<span data-ttu-id="63743-267">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="63743-267">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-beta)
- [<span data-ttu-id="63743-268">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="63743-268">appRoleAssignment</span></span>](/graph/api/resources/approleassignment?view=graph-rest-1.0)
- [<span data-ttu-id="63743-269">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="63743-269">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)
- [<span data-ttu-id="63743-270">application</span><span class="sxs-lookup"><span data-stu-id="63743-270">application</span></span>](/graph/api/resources/application?view=graph-rest-1.0)
- [<span data-ttu-id="63743-271">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="63743-271">claimsMappingPolicy</span></span>](https://docs.microsoft.com/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)
- [<span data-ttu-id="63743-272">keyCredential</span><span class="sxs-lookup"><span data-stu-id="63743-272">keyCredential</span></span>](/graph/api/resources/keycredential?view=graph-rest-1.0)
