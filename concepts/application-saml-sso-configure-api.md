---
title: Use as APIs do Microsoft Graph para configurar o logon único baseado em SAML
description: Aprenda a economizar tempo usando as APIs do Microsoft Graph para automatizar a configuração de logon único baseado em SAML.
author: kenwith
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: b4e2c02fb5583febdaee7eb2e20bca7083b32635
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567464"
---
# <a name="automate-saml-based-sso-app-configuration-with-microsoft-graph-api"></a>Automação da configuração do aplicativo de SSO baseado em SAML com o Microsoft Graph API

Neste artigo, você aprenderá a criar e configurar um aplicativo da galeria do Azure Active Directory (Azure AD). Esse artigo usa o AWS como exemplo, mas você pode usar as etapas neste artigo para qualquer aplicativo baseado em SAML na galeria do Azure AD.

**Etapas para usar as APIs do Microsoft Graph para automatizar a configuração de logon único baseado em SAML**

| Etapa  | Detalhes  |
|---------|---------|
| [1. Criar o aplicativo galeria](#step-1-create-the-gallery-application) | Entrar no cliente da API <br> Recuperar o aplicativo galeria <br> Criar o aplicativo galeria|
| [2. Configurar o logon único](#step-2-configure-single-sign-on) | Recuperar ID de objeto do aplicativo e ID do objeto da entidade de serviço <br> Definir o modo de logon único <br> Definir URLs SAML básicas, como identificador, URL de resposta, URL de logon <br> Adicionar funções de aplicativo (opcional)|
| [3. Configurar mapeamento de declarações](#step-3-configure-claims-mapping) | Criar política de mapeamento de declarações <br> Atribuir política de mapeamento de declarações à entidade de serviço|
| [4. Configurar o certificado de autenticação](#step-4-configure-signing-certificate) | Criar um certificado <BR> Adicionar uma chave de assinatura personalizada <br> Adicionar a chave de assinatura personalizada|
| [5. Atribuir usuários](#step-5-assign-users) | Atribuir usuários e grupos ao aplicativo
| [6. Configurar o lado do aplicativo](#step-6-configure-the-application-side)| Obter os metadados do SAML do Azure AD

**Lista de todas as APIs usadas na documentação**

Verifique se você tem as permissões correspondentes para chamar as seguintes APIs.

|Tipo de recurso |Método |
|---------|---------|
|[applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta)|[Lista applicationTemplate](https://docs.microsoft.com/graph/api/applicationtemplate-list?view=graph-rest-beta&tabs=http) <br>[Instanciar o applicationtemplate](https://docs.microsoft.com/graph/api/applicationtemplate-instantiate?view=graph-rest-beta&tabs=http)|
|[servicePrincipals](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[Atualizar servicePrincipal](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [Criar appRoleAssignments](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-1.0&tabs=http) <br> [Atribuir claimsMappingPolicy](https://docs.microsoft.com/graph/api/serviceprincipal-post-claimsmappingpolicies?view=graph-rest-beta&tabs=http)|
|[aplicativos](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)|[Atualizar aplicativo](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-1.0&tabs=http)|
|[claimsMappingPolicy](https://docs.microsoft.com/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)| [Criar claimsMappingPolicy](https://docs.microsoft.com/graph/api/claimsmappingpolicy-post-claimsmappingpolicies?view=graph-rest-beta&tabs=http)

>[!NOTE]
>Os objetos de resposta mostrados neste artigo podem ser reduzidos para facilitar a leitura. Todas as propriedades serão retornadas de uma chamada real.

## <a name="step-1-create-the-gallery-application"></a>Etapa 1: Criar o aplicativo galeria

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a>Entrar no Microsoft Graph Explorer (recomendado), no Postman ou em qualquer outro cliente de API que você usa

1. Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer)
2. Selecione **Entrar com a Microsoft** e entre usando as credenciais de administrador global do Azure AD ou de Administrador do Aplicativo.
3. Uma vez acessado, você verá os detalhes da conta do usuário no painel esquerdo.

### <a name="retrieve-the-gallery-application-template-identifier"></a>Recuperar o identificador de modelos de aplicativo de galeria

Os aplicativos na galeria do aplicativo do Azure AD têm um [modelo de aplicativo](https://docs.microsoft.com/graph/api/applicationtemplate-list?view=graph-rest-beta&tabs=http) cada um, que descreve os metadados para esse aplicativo. Usando esse modelo, você pode criar uma instância do aplicativo e da entidade de serviço no locatário para gerenciamento.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
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
             "developerServices"
         ],
         "publisher": "Amazon",
         "description": null    
  
}
```

### <a name="create-the-gallery-application"></a>Criar o aplicativo galeria

Usando a ID do modelo que você recuperou para o aplicativo na última etapa, [criar uma instância](https://docs.microsoft.com/graph/api/applicationtemplate-instantiate?view=graph-rest-beta&tabs=http) do aplicativo e da entidade de serviço em seu locatário.

> [!NOTE] 
> Você pode usar a API applicationTemplate para criar uma instância [aplicativos Não-Galeria](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal). Usar o applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.

> [!NOTE]
> Aguarde algum tempo para que o aplicativo seja provisionado em seu locatário do Azure AD. Não é instantâneo. Uma estratégia é fazer uma consulta GET sobre o objeto do aplicativo/entidade de serviço a cada 5-10 segundos até que a consulta seja bem-sucedida.


#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```

#### <a name="response"></a>Resposta


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json


{
    "application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63",
        "appId": "92653dd4-aa3a-3323-80cf-e8cfefcc8d5d",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "AWS Contoso",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "logoutUrl": null,
        "samlMetadataUrl": null,
    },
    "servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e",
        "appDisplayName": "AWS Contoso",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "appRoleAssignmentRequired": true,
        "displayName": "My custom name",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "servicePrincipalNames": [
            "93653dd4-aa3a-4323-80cf-e8cfefcc8d7d"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp"
        ],
    }
}
```

## <a name="step-2-configure-single-sign-on"></a>2. Configurar o logon único

### <a name="retrieve-app-object-id-and-service-principal-object-id"></a>Recuperar ID de objeto do aplicativo e ID do objeto da entidade de serviço

Use a resposta da chamada anterior para recuperar e salvar a ID de objeto do aplicativo e a ID do objeto da entidade de serviço.

```
"application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63"
}
"servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```
### <a name="set-single-sign-on-mode"></a>Definir o modo de logon único

Neste exemplo, você definirá o `saml` como o modo de logon único na [tipo de recurso de servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0). Outras propriedades de SSO do SAML que você pode configurar são: `notificationEmailAddresses`, `loginUrl`e `samlSingleSignOnSettings.relayState`

Antes dessa consulta funcionar, você precisará fornecer consentimento na guia **Modificar permissões** no Graph Explorer. Além disso, certifique-se de que você está usando a ID do** servicePrincipal** obtida anteriormente.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: servicePrincipal/json

{
    "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls-such-as-identifier-reply-url-sign-on-url"></a>Definir URLs SAML básicas, como identificador, URL de resposta, URL de logon

Defina o identificador e as URLs de resposta para AWS no objeto do aplicativo.

 Verifique se você está usando a ID de **aplicativo** obtida anteriormente.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/applications/cbc071a6-0fa5-4859-8g55-e983ef63df63
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

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204
```
### <a name="add-app-roles-optional"></a>Adicionar funções de aplicativo (opcional)

Se o aplicativo exigir as informações da função no token, adicione a definição das funções no objeto do aplicativo. No AWS, você pode [habilitar o provisionamento de usuário](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api) para buscar todas as funções dessa conta do AWS. 

Para saber mais, leia [Configurar a declaração de função emitida no token SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)

> [!NOTE] 
> Ao adicionar funções de aplicativo, não modifique as funções de aplicativo padrão msiam_access. 

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/serviceprincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
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

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a>3. Configurar mapeamento de declarações

### <a name="create-claims-mapping-policy"></a>Criar política de mapeamento de declarações

Além das declarações básicas, configure as seguintes declarações para o Azure AD emitir no token SAML:

| Nome da declaração | Origem  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | assignedroles| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | userprincipalname |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | "900" |
| funções | assignedroles |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | userprincipalname |

Para obter mais informações, confira [Personalizar as declarações emitidas no token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).

> [!NOTE]
> Algumas chaves na política de mapeamento de declarações diferenciam maiúsculas de minúsculas (por exemplo, "Version"). Se você receber uma mensagem de erro como "A propriedade tem um valor inválido", pode ser um problema de diferenciação de maiúsculas e minúsculas.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: claimsMappingPolicies/json

{
    "definition":[
            "{\"ClaimsMappingPolicy\": {
                \"Version\": 1,
                \"IncludeBasicClaimSet\": \"true\",
                \"ClaimsSchema\": [
                    {
                        \"Source\": \"user\",
                        \"ID\": \"assignedroles\",
                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"userprincipalname\",
                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"900\",
                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"assignedroles\",
                        \"SamlClaimType\": \"appRoles\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"userprincipalname\",
                        \"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"
                    }
                ]
            }
        }"

    ],
    "displayName": "AWS Claims policy",
    "isOrganizationDefault": false
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicies",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: claimsMappingPolicies/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
    "id": "6b33aa8e-51f3-41a6-a0fd-d660d276197a",
    "definition": [
        "{\"ClaimsMappingPolicy\": {\"Version\": 1,\"IncludeBasicClaimSet\": \"true\",\"ClaimsSchema\": [{\"Source\": \"user\",\"ID\": \"assignedroles\",\"SamlClaimType\":\"https://aws.amazon.com/SAML/Attributes/Role\"\r\n                    },{\"Source\": \"user\",\"ID\": \"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"},{\"Source\": \"user\",\"ID\": \"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"},{\"Source\": \"user\",\"ID\": \"assignedroles\",\"SamlClaimType\":\"appRoles\"},{\"Source\": \"user\",\"ID\": \"userprincipalname\",\"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims policy",
    "isOrganizationDefault": false
}
```

### <a name="assign-claims-mapping-policy-to-service-principal"></a>Atribuir política de mapeamento de declarações à entidade de serviço

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/claimsMappingPolicies/$ref

Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/6b33aa8e-51f3-41a6-a0fd-d660d276197a"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-4-configure-signing-certificate"></a>Etapa 4. Configurar o certificado de autenticação

Usar a API [applicationtemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) não cria um certificado de autenticação por padrão. Crie seu certificado de assinatura personalizado e atribua-o ao aplicativo. 

### <a name="create-a-custom-signing-certificate"></a>Criar um certificado de autenticação personalizado

Para testar, use o seguinte comando do Windows PowerShell para obter um certificado autoassinado. Você precisará manipular e extrair os valores necessários manualmente usando outras ferramentas. Use a prática recomendada de segurança da sua empresa para criar um certificado de autenticação para produção.

```powershell
Param(
    [Parameter(Mandatory=$true)]
    [string]$fqdn,
    [Parameter(Mandatory=$true)]
    [string]$pwd,
    [Parameter(Mandatory=$true)]
    [string]$location
) 

if (!$PSBoundParameters.ContainsKey('location'))
{
    $location = "."
} 

$cert = New-SelfSignedCertificate -certstorelocation cert:\currentuser\my -DnsName $fqdn
$pwdSecure = ConvertTo-SecureString -String $pwd -Force -AsPlainText
$path = 'cert:\currentuser\my\' + $cert.Thumbprint
$cerFile = $location + "\\" + $fqdn + ".cer"
$pfxFile = $location + "\\" + $fqdn + ".pfx" 

Export-PfxCertificate -cert $path -FilePath $pfxFile -Password $pwdSecure
Export-Certificate -cert $path -FilePath $cerFile
```

Como alternativa, o seguinte aplicativo de console C# pode ser usado como Prova de Conceito para entender como os valores necessários podem ser obtidos. Observe que este código é para **aprendizado e referência APENAS** e não devem ser usados como estão na produção.

```csharp
using System;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;
using System.Text;


/* CONSOLE APP - PROOF OF CONCEPT CODE ONLY!!
 * This code uses a self signed certificate and should not be used 
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
            Console.WriteLine("For All startDateTime: " + startDate.ToString("o"));

            // Print out the end date in ISO 8601 format.
            DateTime endDate = DateTime.Parse(selfsignedCert.GetExpirationDateString()).ToUniversalTime();
            Console.WriteLine("For All endDateTime: " + endDate.ToString("o"));

            // Print the GUID used for keyId
            string signAndPasswordGuid = Guid.NewGuid().ToString();
            string verifyGuid = Guid.NewGuid().ToString();
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Sign and passwordCredentials: " + signAndPasswordGuid);
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Verify: " + verifyGuid);

            // Print out the password.
            Console.WriteLine("Password is: {0}", password);

            // Print out a displayName to use as an example.
            Console.WriteLine("displayName to use: CN=Example");
            Console.WriteLine();

            // Print out the public key.
            Console.WriteLine("Public Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Cert)), Environment.NewLine);
            Console.WriteLine();

            // Generate the customKeyIdentifier using hash of thumbprint.
            Console.WriteLine("You can generate the customKeyIdentifier by getting the SHA256 hash of the certs thumprint.\nThe certs thumbprint is: {0}{1}", selfsignedCert.Thumbprint, Environment.NewLine);
            Console.WriteLine("The hash of the thumbprint that we will use for customeKeyIdentifier is:");
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

                request.CertificateExtensions.Add(
                    new X509KeyUsageExtension(X509KeyUsageFlags.DataEncipherment | X509KeyUsageFlags.KeyEncipherment | X509KeyUsageFlags.DigitalSignature, false));

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

### <a name="add-a-custom-signing-key"></a>Adicionar uma chave de assinatura personalizada

Adicione as seguintes informações à entidade de serviço:

* Chave privada
* Senha
* Chave pública 

Extraia a chave pública e privada Base64 do arquivo PFX. Para saber mais sobre as propriedades, leia [tipo de recurso de keyCredential](https://docs.microsoft.com/graph/api/resources/keycredential?view=graph-rest-1.0).

Certifique-se de que a keyId da keyCredential usada para "Assinar" corresponda à keyId da passwordCredential. Você pode gerar o `customkeyIdentifier` ao obter o hash da impressão digital do certificado. Confira o código de referência do C# acima.

#### <a name="request"></a>Solicitação

> [!NOTE]
> O valor "chave" na propriedade keyCredentials é reduzido para facilitar a leitura. O valor é base 64 codificado. Para a chave particular, a propriedade `usage` é "Assinar". Para a chave pública, a propriedade `usage` é "Verificar".

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: servicePrincipals/json

{
    "keyCredentials":[
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "X509CertAndPassword",
            "usage": "Sign",
            "key":"MIIKIAIBAz.....HBgUrDgMCERE20nuTptI9MEFCh2Ih2jaaLZBZGeZBRFVNXeZmAAgIH0A==",
            "displayName": "CN=awsAPI"
        },
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "e35a7d11-fef0-49ad-9f3e-aacbe0a42c42",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "AsymmetricX509Cert",
            "usage": "Verify",
            "key": "MIIDJzCCAg+gAw......CTxQvJ/zN3bafeesMSueR83hlCSyg==",
            "displayName": "CN=awsAPI"
        }

    ],
    "passwordCredentials": [
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "endDateTime": "2022-01-27T19:40:33Z",
            "startDateTime": "2020-04-20T19:40:33Z",
            "secretText": "61891f4ee44d"
        }
    ]
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a>Adicionar a chave de assinatura personalizada

É necessário definir a propriedade `preferredTokenSigningKeyThumbprint` como a impressão digital do certificado que você deseja que o Azure AD use para assinar a resposta SAML. 

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: servicePrincipals/json

{
    "preferredTokenSigningKeyThumbprint": "AC09FEF18DDE6983EE2A164FBA3C4DD7518BD787"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```
## <a name="step-5-assign-users"></a>Etapa 5. Atribuir usuários

### <a name="assign-users-and-groups-to-the-application"></a>Atribuir usuários e grupos ao aplicativo

Atribua o seguinte usuário à entidade de serviço e atribua o AWS_Role1. 

| Nome  | ID  |
|---------|---------|
| ID de usuário (principalId) | 6cad4079-4e79-4a3f-9efb-ea30a14bdb26 |
| Type (principalType) | Usuário |
| ID da função do aplicativo (appRoleId) | 454dc4c2-8176-498e-99df-8c4efcde41ef |
| servicePrincipalID (resourceId) | f47a6776-bca7-4f2e-bc6c-eec59d058e3e |

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
  "principalType": "User",
  "appRoleId":"454dc4c2-8176-498e-99df-8c4efcde41ef",
  "resourceId":"f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```
#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

{
    "id": "rq7hyzl4yECaNZleMrTpDV-OCe5TEl5Ao_o76XMrRFU",
    "creationTimestamp": "2020-04-23T17:38:13.2508567Z",
    "appRoleId": "454dc4c2-8176-498e-99df-8c4efcde41ef",
    "principalDisplayName": "User 1",
    "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
    "principalType": "User",
    "resourceDisplayName": "AWS API Created",
    "resourceId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```

Para saber mais, confira o tipo de recurso [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-1.0).

## <a name="step-6-configure-the-application-side"></a>Etapa 6. Configurar o lado do aplicativo

### <a name="get-azure-ad-saml-metadata"></a>Obter os metadados do SAML do Azure AD

Use a URL a seguir para obter os metadados do SAML do Azure AD para o aplicativo específico configurado. Os metadados contêm informações como o certificado de assinatura, o Azure AD entityID e o Azure AD SingleSignOnService, entre outras.

https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}

## <a name="next-steps"></a>Próximas etapas
- [Use as APIs do Microsoft Graph para configurar o provisionamento de usuário](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api)
- [Use o relatório de atividade do aplicativo AD FS para migrar aplicativos para o Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-application-activity)
