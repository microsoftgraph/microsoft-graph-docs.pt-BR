---
title: Use as APIs do Microsoft Graph para configurar o logon único baseado em SAML
description: Aprenda a economizar tempo usando as APIs do Microsoft Graph para automatizar a configuração de logon único baseado em SAML.
author: kenwith
localization_priority: Priority
ms.custom: scenarios:getting-started
ms.prod: applications
ms.openlocfilehash: 53fa3b995b630837f27b9ebaf9a30825f4bccf4c5efd49b7b6e85034e55985dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54151963"
---
# <a name="configure-saml-based-single-sign-on-for-your-application-using-the-microsoft-graph-api"></a>Configure o logon único baseado em SAML para seu aplicativo usando a API do Microsoft Graph

Neste artigo, você aprenderá como criar e configurar um SSO (logon único) baseado em SAML para seu aplicativo no Azure AD (Azure Active Directory) usando a API do Microsoft Graph. A configuração do aplicativo inclui URLs básicas de SAML, uma política de mapeamento de declarações e o uso de um certificado para adicionar uma chave de assinatura personalizada. Após o aplicativo ser criado, atribua a ele um usuário como administrador. Em seguida, você pode usar uma URL para obter metadados SAML do Azure AD para configuração adicional do aplicativo. 

Este artigo usa um modelo de aplicativo Azure AD da AWS como exemplo, mas você pode usar as etapas deste artigo para qualquer aplicativo baseado em SAML na Galeria do Azure AD.

## <a name="prerequisites"></a>Pré-requisitos

Este tutorial assume que você está usando o Microsoft Graph Explorer, mas você pode usar o Postman ou criar seu próprio aplicativo cliente para chamar o Microsoft Graph. Para chamar as APIs do Microsoft Graph neste tutorial, você precisa usar uma conta com a função de administrador global e as permissões apropriadas. Para este tutorial, as permissões delegadas `Application.ReadWrite.All`,`AppRoleAssignment.ReadWrite.All`,`Policy.Read.All`,`Policy.ReadWrite.ApplicationConfiguration` e `User.ReadWrite.All` são necessárias. Conclua as seguintes etapas para definir as permissões no Microsoft Graph Explorer:

1. Vá para o [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
2. Selecione **Entrar com a conta da Microsoft** e entre usando uma conta de administrador global do Azure AD. Uma vez acessado, você verá os detalhes da conta do usuário no painel esquerdo.
3. Selecione o ícone de configurações à direita dos detalhes da conta do usuário e, em seguida, selecione **Selecionar permissões**.

    ![Selecionar as permissões do Microsoft Graph](./images/application-saml-sso-configure-api/set-permissions.png)
        
4. Na lista de permissões, role e expanda **AppRoleAssignment (1)** e selecione a permissão **AppRoleAssignment.ReadWrite.All**. Role mais para baixo e expanda **Aplicativo (2)** e selecione a permissão **Application.ReadWrite.All**. Continue e expanda **Política (13)** e, em seguida, selecione as permissões **Policy.Read.All**  e **Policy.ReadWrite.ApplicationConfiguration**. Por fim, role e expanda **Usuários (8)** e selecione **User.ReadWrite.All**.

    ![Rolar e selecionar as permissões approleassignment, application e policy ](./images/application-saml-sso-configure-api/select-permissions.png)

5. Selecione **Consentimento** e, em seguida, selecione **Aceitar** para aceitar o consentimento das permissões. Você não precisa consentir em nome da organização para essas permissões.

    ![Aceitar o consentimento das permissões](./images/application-saml-sso-configure-api/accept-permissions.png)

## <a name="step-1-create-the-application"></a>Etapa 1: Criar o aplicativo

O Azure AD tem uma galeria que contém milhares de aplicativos pré-integrados que você pode usar como modelo para seu aplicativo. O modelo de aplicativo descreve os metadados para o aplicativo. Usando esse modelo, você pode criar uma instância do aplicativo e da entidade de serviço no locatário para gerenciamento. 

Para criar o aplicativo a partir da galeria, primeiro obtenha o identificador do modelo de aplicativo e, em seguida, use esse identificador para criar o aplicativo.

### <a name="retrieve-the-gallery-application-template-identifier"></a>Recuperar o identificador do modelo de aplicativo da galeria

 Neste tutorial, recupere o identificador do modelo de aplicativo para `AWS Single Sign-on`. Registre o valor da propriedade **id** para usar posteriormente neste tutorial.

#### <a name="request"></a>Solicitação

```http
GET https://graph.microsoft.com/v1.0/applicationTemplates?$filter=displayName eq 'AWS Single Sign-on'
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applicationTemplates",
  "value": [
    {
      "id": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
      "displayName": "AWS Single Sign-on",
      "homePageUrl": "https://aws.amazon.com/",
      "supportedSingleSignOnModes": [
        "saml",
        "external"
      ],
      "supportedProvisioningTypes": [
        "sync"
      ],
      "logoUrl": "https://az495088.vo.msecnd.net/app-logo/awssinglesignon_215.png",
      "categories": [
        "developerServices",
        "itInfrastructure",
        "security",
        "New"
      ],
      "publisher": "Amazon Web Services, Inc.",
      "description": "Federate once to AWS SSO & use it to manage access centrally to multiple AWS accounts. Provision users via SCIM & get Azure AD single sign-in access to the AWS Console, CLI, & AWS SSO integrated apps."
    }
  ]
}
```

### <a name="create-the-application"></a>Criar o aplicativo

Usando o valor **id** registrado para o modelo de aplicativo, crie uma instância do aplicativo e da entidade de serviço no locatário. Registre o valor da propriedade **id** do aplicativo e o valor da propriedade **id** para o principal de serviço usar posteriormente neste tutorial.

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/21ed01d2-ec13-4e9e-86c1-cd546719ebc4/instantiate
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.applicationServicePrincipal",
  "application": {
    "id": "a9be408a-6c31-4141-8cea-52fcd4a61be8",
    "appId": "17cad0e7-cd2b-4e51-a75d-ba810f3e4045",
    "applicationTemplateId": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
    "createdDateTime": "2021-05-10T20:12:03Z",
    "deletedDateTime": null,
    "displayName": "AWS Contoso",
    "groupMembershipClaims": null,
    "identifierUris": [],
    "isFallbackPublicClient": false,
    "signInAudience": "AzureADMyOrg",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "defaultRedirectUri": null,
    "optionalClaims": null,
    "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
    },
    "addIns": [],
    "api": {
      "acceptMappedClaims": null,
      "knownClientApplications": [],
      "requestedAccessTokenVersion": null,
      "oauth2PermissionScopes": [
        {
          "adminConsentDescription": "Allow the application to access AWS Contoso on behalf of the signed-in user.",
          "adminConsentDisplayName": "Access AWS Contoso",
          "id": "6f891cd3-c132-4822-930b-f343b4515d19",
          "isEnabled": true,
          "type": "User",
          "userConsentDescription": "Allow the application to access AWS Contoso on your behalf.",
          "userConsentDisplayName": "Access AWS Contoso",
          "value": "user_impersonation"
        }
      ],
      "preAuthorizedApplications": []
    },
    "appRoles": [
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "User",
        "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
        "isEnabled": true,
        "description": "User",
        "value": null,
        "origin": "Application"
      },
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "msiam_access",
        "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
        "isEnabled": true,
        "description": "msiam_access",
        "value": null,
        "origin": "Application"
      }
    ],
    "info": {
      "logoUrl": null,
      "marketingUrl": null,
      "privacyStatementUrl": null,
      "supportUrl": null,
      "termsOfServiceUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
      "countriesBlockedForMinors": [],
      "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "publicClient": {
      "redirectUris": []
    },
    "requiredResourceAccess": [],
    "web": {
      "homePageUrl": "https://*.signin.aws.amazon.com/platform/saml/acs/*?metadata=awssinglesignon|ISV9.1|primary|z",
      "redirectUris": []
    }
  },
  "servicePrincipal": {
    "id": "a750f6cf-2319-464a-bcc3-456926736a91",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appId": "17cad0e7-cd2b-4e51-a75d-ba810f3e4045",
    "applicationTemplateId": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
    "appDisplayName": "AWS Contoso",
    "alternativeNames": [],
    "appOwnerOrganizationId": "8500cad3-193d-48a6-8d00-c129b114dc10",
    "displayName": "AWS Contoso",
    "appRoleAssignmentRequired": true,
    "loginUrl": null,
    "logoutUrl": null,
    "homepage": "https://*.signin.aws.amazon.com/platform/saml/acs/*?metadata=awssinglesignon|ISV9.1|primary|z",
    "notificationEmailAddresses": [],
    "preferredSingleSignOnMode": null,
    "preferredTokenSigningKeyThumbprint": null,
    "replyUrls": [],
    "servicePrincipalNames": [
      "17cad0e7-cd2b-4e51-a75d-ba810f3e4045"
    ],
    "servicePrincipalType": "Application",
    "tags": [
      "WindowsAzureActiveDirectoryIntegratedApp"
    ],
    "tokenEncryptionKeyId": null,
    "samlSingleSignOnSettings": null,
    "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
    },
    "addIns": [],
    "appRoles": [
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "User",
        "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
        "isEnabled": true,
        "description": "User",
        "value": null,
        "origin": "Application"
      },
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "msiam_access",
        "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
        "isEnabled": true,
        "description": "msiam_access",
        "value": null,
        "origin": "Application"
      }
    ],
    "info": {
      "logoUrl": null,
      "marketingUrl": null,
      "privacyStatementUrl": null,
      "supportUrl": null,
      "termsOfServiceUrl": null
    },
    "keyCredentials": [],
    "oauth2PermissionScopes": [
      {
        "adminConsentDescription": "Allow the application to access AWS Contoso on behalf of the signed-in user.",
        "adminConsentDisplayName": "Access AWS Contoso",
        "id": "6f891cd3-c132-4822-930b-f343b4515d19",
        "isEnabled": true,
        "type": "User",
        "userConsentDescription": "Allow the application to access AWS Contoso on your behalf.",
        "userConsentDisplayName": "Access AWS Contoso",
        "value": "user_impersonation"
      }
    ],
    "passwordCredentials": []
  }
}
```

## <a name="step-2-configure-single-sign-on"></a>2. Configurar o logon único

Neste tutorial, defina `saml` como modo de logon único na entidade de serviço. Use o **id** do principal de serviço que você registrou anteriormente.

#### <a name="request"></a>Solicitação

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91
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

Usando o **id** para o aplicativo que você registrou anteriormente, defina o URI do identificador e redirecione o URI para a AWS no objeto do aplicativo.

#### <a name="request"></a>Solicitação

```http
PATCH https://graph.microsoft.com/v1.0/applications/a9be408a-6c31-4141-8cea-52fcd4a61be8
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

Use o **id** do principal de serviço que você registrou anteriormente.

#### <a name="request"></a>Solicitação

```http
PATCH https://graph.microsoft.com/v1.0/serviceprincipals/a9be408a-6c31-4141-8cea-52fcd4a61be8
Content-type: serviceprincipals/json

{
  "appRoles": [
    {
      "allowedMemberTypes": [
        "User"
      ],
      "displayName": "User",
      "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
      "isEnabled": true,
      "description": "User",
      "value": null,
      "origin": "Application"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "displayName": "msiam_access",
      "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
      "isEnabled": true,
      "description": "msiam_access",
      "value": null,
      "origin": "Application"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Admin,WAAD",
      "displayName": "Admin,WAAD",
      "id": "3a84e31e-bffa-470f-b9e6-754a61e4dc63",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Finance,WAAD",
      "displayName": "Finance,WAAD",
      "id": "7a960000-ded3-455b-8c04-4f2ace00319b",
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
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
  "id": "a4b35718-fd5e-4ca8-8248-a3c9934b1b78",
  "deletedDateTime": null,
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
  ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

### <a name="assign-a-claims-mapping-policy-to-a-service-principal"></a>Atribuir uma política de mapeamento de declarações a uma entidade de serviço

Use o **id** do principal de serviço que você registrou anteriormente para atribuir uma política de mapeamento de declarações a ele. Use o valor da propriedade **id** para a política de mapeamento de declarações no corpo da solicitação.

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/claimsMappingPolicies/$ref
Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/a4b35718-fd5e-4ca8-8248-a3c9934b1b78"
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204
```

## <a name="step-4-configure-a-signing-certificate"></a>Etapa 4. Configurar um certificado de autenticação

Neste tutorial, você precisa de um certificado autoassinado que o Azure Active Directory pode usar para assinar uma resposta SAML. Você pode usar seu próprio certificado ou pode usar o exemplo a seguir. 

### <a name="create-a-signing-certificate"></a>Criar um certificado de assinatura

Usando o **id** do principal de serviço que você criou, crie um novo certificado e inclua-o no principal de serviço.

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=AWSContoso",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "p9PEYmuKhP2oaMzGfSdNQC/9ChA=",
  "displayName": "CN=AWSContoso",
  "endDateTime": "2024-01-25T00:00:00Z",
  "key": "MIICqjCCAZKgAwIBAgIId....4rnrk43wp75yqjRbOhAZ1ExAxVqW+o2JslhjUeltUMNQW+ynOfs9oHu1ZdnGmxrE=",
  "keyId": "70883316-50be-4016-ba80-19d9fbad873d",
  "startDateTime": "2021-05-10T20:35:37.5754318Z",
  "thumbprint": "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10",
  "type": "AsymmetricX509Cert",
  "usage": "Verify"
}
```

### <a name="activate-the-custom-signing-key"></a>Adicionar a chave de assinatura personalizada

É necessário definir a propriedade **preferredTokenSigningKeyThumbprint** da entidade de serviço para a impressão digital do certificado que você deseja que o Azure AD use para assinar a resposta SAML. 

#### <a name="request"></a>Solicitação

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91
Content-type: servicePrincipals/json

{
  "preferredTokenSigningKeyThumbprint": "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10"
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
  "id": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "MyTestUser1@contoso.com"
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
POST https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/appRoleAssignments
Content-type: appRoleAssignments/json

{
  "principalId": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "principalType": "User",
  "appRoleId":"3a84e31e-bffa-470f-b9e6-754a61e4dc63",
  "resourceId":"a750f6cf-2319-464a-bcc3-456926736a91"
}
```

#### <a name="response"></a>Resposta

```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('a750f6cf-2319-464a-bcc3-456926736a91')/appRoleAssignments/$entity",
  "id": "mZUPBA98lE-qdYOUxMbqm2qY3odGRGdFtpYJkAfUC0Q",
  "deletedDateTime": null,
  "appRoleId": "3a84e31e-bffa-470f-b9e6-754a61e4dc63",
  "createdDateTime": "2021-05-10T21:04:11.0480851Z",
  "principalDisplayName": "MyTestUser1",
  "principalId": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "principalType": "User",
  "resourceDisplayName": "AWS Contoso",
  "resourceId": "a750f6cf-2319-464a-bcc3-456926736a91"
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
DELETE https://graph.microsoft.com/v1.0/applications/a9be408a-6c31-4141-8cea-52fcd4a61be8
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

### <a name="delete-the-user-account"></a>Excluir a conta de usuário

Exclua a conta de usuário MyTestUser1.

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/v1.0/users/040f9599-7c0f-4f94-aa75-8394c4c6ea9b
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

### <a name="delete-the-claims-mapping-policy"></a>Excluir a política de mapeamento de declarações

Exclua a política de mapeamento de declarações.

#### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/a4b35718-fd5e-4ca8-8248-a3c9934b1b78
```

#### <a name="response"></a>Resposta

```http
No Content - 204
```

## <a name="see-also"></a>Confira também

- No AWS, você pode [habilitar o provisionamento de usuário](/azure/active-directory/app-provisioning/application-provisioning-configure-api) para buscar todas as funções dessa conta do AWS. Para saber mais, confira [Configurar a declaração de função emitida no token SAML](/azure/active-directory/develop/active-directory-enterprise-app-role-management).
- [Personalizar as declarações emitidas em tokens para um aplicativo específico em um locatário](/azure/active-directory/develop/active-directory-claims-mapping).
- Você pode usar a API applicationTemplate para criar uma instância [Aplicativos inexistentes na galeria](/azure/active-directory/manage-apps/view-applications-portal). Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.
- [applicationTemplate](/graph/api/resources/applicationtemplate)
- [appRoleAssignment](/graph/api/resources/approleassignment)
- [servicePrincipal](/graph/api/resources/serviceprincipal)
- [application](/graph/api/resources/application)
- [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy)
- [keyCredential](/graph/api/resources/keycredential)
- [addTokenSigningCertificate](/graph/api/serviceprincipal-addtokensigningcertificate?view=graph-rest-beta&preserve-view=true)
