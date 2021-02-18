---
title: Use as APIs do Microsoft Graph para configurar o logon único baseado em SAML
description: Aprenda a economizar tempo usando as APIs do Microsoft Graph para automatizar a configuração de logon único baseado em SAML.
author: kenwith
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: 3ab54e4726635262579f3ef54625197f0191c5ae
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272133"
---
# <a name="configure-saml-based-single-sign-on-for-your-application-using-the-microsoft-graph-api"></a>Configure o logon único baseado em SAML para seu aplicativo usando a API do Microsoft Graph

Neste artigo, você aprenderá como criar e configurar um SSO (logon único) baseado em SAML para seu aplicativo no Azure AD (Azure Active Directory) usando a API do Microsoft Graph. A configuração do aplicativo inclui URLs básicas de SAML, uma política de mapeamento de declarações e o uso de um certificado para adicionar uma chave de assinatura personalizada. Após o aplicativo ser criado, atribua a ele um usuário como administrador. Em seguida, você pode usar uma URL para obter metadados SAML do Azure AD para configuração adicional do aplicativo. 

Este artigo usa um modelo de aplicativo Azure AD da AWS como exemplo, mas você pode usar as etapas deste artigo para qualquer aplicativo baseado em SAML na Galeria do Azure AD.

>[!NOTE]
>As chaves e os objetos de resposta mostrados neste artigo poderiam ser reduzidos para facilitar a leitura.

## <a name="prerequisites"></a>Pré-requisitos

- Neste tutorial, você precisa de um certificado autoassinado que o Azure AD pode usar para assinar uma resposta SAML. Você pode usar seu próprio certificado ou usar algo como o seguinte código C# para criar um certificado de teste:

    > **Observação** Este código é **APENAS** para aprendizado e referência, e não deve ser usado como está na produção.

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

    Para concluir este tutorial, registre os seguintes valores do seu certificado:

    - Chave privada
    - Data e hora de início
    - Data e hora de término
    - Senha do certificado
    - Nome de exibição
    - Chave pública
    - Hash da impressão digital
    - Identificador de chave

    Além dos valores do certificado, também serão necessários dois novos GUIDS para os keyIds usados. O exemplo a seguir mostra a saída do código listado anteriormente:

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

- Este tutorial assume que você está usando o Microsoft Graph Explorer, mas você pode usar o Postman ou criar seu próprio aplicativo cliente para chamar o Microsoft Graph. Para chamar as APIs do Microsoft Graph neste tutorial, você precisa usar uma conta com a função de administrador global e as permissões apropriadas. Para este tutorial, serão necessárias as permissões delegadas `Application.ReadWrite.All`, `AppRoleAssignment.ReadWrite.All`, `Policy.Read.All` e`Policy.ReadWrite.ApplicationConfiguration`. Conclua as seguintes etapas para definir as permissões no Microsoft Graph Explorer:

    1. Inicie o [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
    2. Selecione **Entrar com a conta da Microsoft** e entre usando uma conta de administrador global do Azure AD. Uma vez acessado, você verá os detalhes da conta do usuário no painel esquerdo.
    3. Selecione o ícone de configurações à direita dos detalhes da conta do usuário e, em seguida, selecione **Selecionar permissões**.

        ![Selecionar as permissões do Microsoft Graph](./images/application-saml-sso-configure-api/set-permissions.png)
        
    4. Role pela lista de permissões até permissões de `AppRoleAssignment`, expanda **AppRoleAssignment (1)** e selecione a permissão **AppRoleAssignment.ReadWrite.All**. Role ainda mais para baixo pela lista de permissões de `Application`, expanda **Application (2)** e selecione a permissão **Application.ReadWrite.All**. Continue até permissões de `Policy`, expanda **Policy (13)**, e selecione as permissões **Policy.Read.All** e **Policy.ReadWrite.ApplicationConfiguration**.

        ![Rolar e selecionar as permissões approleassignment, application e policy ](./images/application-saml-sso-configure-api/select-permissions.png)

    5. Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões. Você não precisa consentir em nome da organização para essas permissões.

        ![Aceitar o consentimento das permissões](./images/application-saml-sso-configure-api/accept-permissions.png)

## <a name="step-1-create-the-application"></a>Etapa 1: Criar o aplicativo

O Azure AD tem uma galeria que contém milhares de aplicativos pré-integrados que você pode usar como modelo para seu aplicativo. O modelo de aplicativo descreve os metadados para o aplicativo. Usando esse modelo, você pode criar uma instância do aplicativo e da entidade de serviço no locatário para gerenciamento. 

Para criar o aplicativo a partir da galeria, primeiro obtenha o identificador do modelo de aplicativo e, em seguida, use esse identificador para criar o aplicativo.

### <a name="retrieve-the-gallery-application-template-identifier"></a>Recuperar o identificador do modelo de aplicativo da galeria

 Neste tutorial, recupere o identificador do modelo de aplicativo para `Amazon Web Services (AWS)`. Registre o valor da propriedade **id** para usar posteriormente neste tutorial.

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/beta/applicationTemplates?$filter=displayName eq 'Amazon Web Services (AWS)'
```

#### <a name="response"></a>Resposta

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

### <a name="create-the-application"></a>Criar o aplicativo

Usando o valor **id** registrado para o modelo de aplicativo, crie uma instância do aplicativo e da entidade de serviço no locatário. Registre o valor da propriedade **objectId** do aplicativo e o valor da propriedade **objectId** para que a entidade de serviço possa usar posteriormente neste tutorial.

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```

> [!NOTE]
> Aguarde algum tempo para que o aplicativo seja provisionado em seu locatário do Azure AD. Não é instantâneo. Uma estratégia é fazer uma consulta GET sobre o objeto de aplicativo e a entidade de serviço a cada 5-10 segundos até que a consulta seja bem-sucedida.

#### <a name="response"></a>Resposta

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

## <a name="step-2-configure-single-sign-on"></a>2. Configurar o logon único

Neste tutorial, defina `saml` como modo de logon único na entidade de serviço. Use o **objectId** para a entidade de serviço gravada anteriormente.

#### <a name="request"></a>Solicitação

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: servicePrincipal/json

{
  "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls"></a>Definir URLs básicas de SAML

Usando o **objetoId** para o aplicativo registrado anteriormente, defina o URI do identificador e redirecione o URI para a AWS no objeto de aplicativo.

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204
```

### <a name="add-app-roles-optional"></a>Adicionar funções de aplicativo (opcional)

Se o aplicativo exigir as informações da função no token, adicione a definição das funções no objeto do aplicativo. 

> [!NOTE] 
> Ao adicionar funções de aplicativo, não modifique as funções de aplicativo padrão `msiam_access`. 

Use o **objectId** para a entidade de serviço gravada anteriormente.

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a>3. Configurar mapeamento de declarações

### <a name="create-a-claims-mapping-policy"></a>Criar uma política de mapeamento de declarações

Além das declarações básicas, configure as seguintes declarações para o Azure AD emitir no token SAML:

| Nome da declaração | Origem  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | assignedroles| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | userprincipalname |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | "900" |
| funções | assignedroles |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | userprincipalname |

> [!NOTE]
> Algumas chaves na política de mapeamento de declarações são sensíveis a letras maiúsculas e minúsculas (por exemplo, "Version"). Se você receber uma mensagem de erro como "A propriedade tem um valor inválido", isso poderia ser um problema de diferenciação de maiúsculas e minúsculas.

Crie a política de mapeamento de declarações e registre o valor da propriedade **id** para usar posteriormente neste tutorial.

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

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

### <a name="assign-a-claims-mapping-policy-to-a-service-principal"></a>Atribuir uma política de mapeamento de declarações a uma entidade de serviço

Use o **objectId** para a entidade de serviço gravada anteriormente, para atribuir uma política de mapeamento de declarações a ela. Use o valor da propriedade **id** para a política de mapeamento de declarações no corpo da solicitação.

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27/claimsMappingPolicies/$ref
Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73"
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204
```

## <a name="step-4-configure-a-signing-certificate"></a>Etapa 4. Configurar um certificado de autenticação

Atribua seu certificado ao aplicativo. 

#### <a name="request"></a>Solicitação

No corpo da solicitação, forneça estes valores:

**keyCredentials – Assinar**

- **customKeyIdentifier** – O hash da impressão digital de certificado.
- **endDateTime** – A data e hora de término do certificado.
- **keyId** – O identificador da credencial. Igual à keyId para a **passwordCredentials**.
- **startDateTime** – A data de início do certificado.
- **key** – A chave privada codificada como base 64 do certificado.
- **displayName** – O nome de exibição das credenciais.

**keyCredentials – Verificar**

- **customKeyIdentifier** – O hash da impressão digital de certificado.
- **endDateTime** – A data e hora de término do certificado.
- **keyId** – O identificador da credencial.
- **startDateTime** – A data de início do certificado.
- **key** – A chave pública codificada como base 64 do certificado.
- **displayName** – O nome de exibição das credenciais.

**passwordCredentials**

- **customKeyIdentifier** – O hash da impressão digital de certificado.
- **keyId** – O identificador da credencial. Igual à keyId para a **keyCredentials – Assinar**.
- **endDateTime** – A data e hora de término do certificado.
- **startDateTime** – A data de início do certificado.
- **secretText** – A senha para o certificado.

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

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a>Adicionar a chave de assinatura personalizada

É necessário definir a propriedade **preferredTokenSigningKeyThumbprint** da entidade de serviço para a impressão digital do certificado que você deseja que o Azure AD use para assinar a resposta SAML. 

#### <a name="request"></a>Solicitação

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27

Content-type: servicePrincipals/json

{
    "preferredTokenSigningKeyThumbprint": "14B73D02E5094675063DF66A42B914DAD71633D7"
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204
```

## <a name="step-5-assign-users"></a>Etapa 5. Atribuir usuários

### <a name="create-a-user-account"></a>Criar uma conta de usuário

Para este tutorial, crie uma conta de usuário que será adicionada ao aplicativo. No corpo da solicitação, altere contoso.com para o nome de domínio do seu locatário. Encontre informações sobre locatários na página de visão geral do Azure Active Directory. Registre o **id** do usuário a ser usado posteriormente neste tutorial.

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

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

### <a name="assign-a-user-to-the-application"></a>Atribuir um usuário ao aplicativo

Atribua o usuário que você criou à entidade de serviço e atribua a função de aplicativo `Admin,WAAD`. 

No corpo da solicitação, forneça estes valores:

- **principalId** – O **id** da conta de usuário que você criou.
- **appRoleId** – O **id** da função de apĺicativo `Admin,WAAD` que você adicionou.
- **resourceId** – A **id** da entidade de serviço.

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

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

## <a name="step-6-get-azure-ad-saml-metadata"></a>Etapa 6: Obter metadados SAML do Azure AD

Use a URL a seguir para obter os metadados do SAML do Azure AD para o aplicativo específico configurado. Os metadados contêm informações como o certificado de assinatura, o Azure AD entityID e o Azure AD SingleSignOnService, entre outras.

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

A seguir, é possível ver um exemplo do que você pode ver no aplicativo:

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

## <a name="step-7-clean-up-resources"></a>Etapa 7: Limpar recursos

Nessa etapa, remova os recursos que criou.


### <a name="delete-the-application"></a>Excluir o aplicativo

Exclua o aplicativo que você criou.

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/beta/applications/4b01f51f-079b-4634-b767-7e19ad502cdb
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

### <a name="delete-the-user-account"></a>Excluir a conta de usuário

Exclua a conta de usuário MyTestUser1.

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/v1.0/users/3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

### <a name="delete-the-claims-mapping-policy"></a>Excluir a política de mapeamento de declarações

Exclua a política de mapeamento de declarações.

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

## <a name="see-also"></a>Confira também

- No AWS, você pode [habilitar o provisionamento de usuário](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api) para buscar todas as funções dessa conta do AWS. Para saber mais, confira [Configurar a declaração de função emitida no token SAML](/azure/active-directory/develop/active-directory-enterprise-app-role-management).
- [Personalizar as declarações emitidas em tokens para um aplicativo específico em um locatário](/azure/active-directory/develop/active-directory-claims-mapping).
- Você pode usar a API applicationTemplate para criar uma instância [Aplicativos inexistentes na galeria](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal). Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.
- [New-SelfSignedCertificate](/powershell/module/pkiclient/new-selfsignedcertificate?view=win10-ps)
- [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-beta)
- [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-1.0)
- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)
- [application](/graph/api/resources/application?view=graph-rest-1.0)
- [claimsMappingPolicy](https://docs.microsoft.com/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)
- [keyCredential](/graph/api/resources/keycredential?view=graph-rest-1.0)
