---
title: Configurar o proxy de aplicativo usando as APIs do Microsoft Graph
description: Configure automaticamente o proxy de aplicativo usando as APIs do Microsoft Graph para fornecer acesso remoto e logon único para aplicativos locais.
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc99857905a0a308f49ddc41bf22da993ca8f1b4
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873101"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a>Automatizar a configuração do proxy de aplicativo usando a API do Microsoft Graph

Neste artigo, você aprenderá a criar e configurar o [proxy de aplicativo](https://aka.ms/whyappproxy) do Azure Active Directory (Azure AD) para um aplicativo. O proxy de aplicativo fornece acesso remoto seguro e logon único em aplicativos Web no local. Depois de configurar o proxy de aplicativo para um aplicativo, os usuários podem acessar seus aplicativos locais por meio de uma URL externa, do portal de meus aplicativos ou de outros portais de aplicativos internos.

Este artigo pressupõe que você já instalou um conector e concluiu os [pré-requisitos](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) para o proxy de aplicativo para que os conectores possam se comunicar com os serviços do Azure AD.

Verifique se você tem as permissões correspondentes para chamar as seguintes APIs.

|Tipo de recurso |Método |
|---------|---------|
|[aplicativos](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [onPremisesPublishing](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [Criar aplicativo](https://docs.microsoft.com/graph/api/application-post-applications?view=graph-rest-beta&tabs=http) <br> [Atualizar aplicativo](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [Adicionar aplicativo ao um conector](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[conector](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [Obter conectores](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[connectorGroup](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [Criar connectorGroup](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [Adicionar conector a connectorGroup](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[servicePrincipals](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[Criar servicePrincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals?view=graph-rest-beta&tabs=http) <br> [Atualizar servicePrincipal](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [Criar appRoleAssignments](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> As solicitações mostradas neste artigo usam valores de amostra. Você precisará atualizá-los. Os objetos Response mostrados também podem ser reduzidos para facilitar a leitura. 

## <a name="step-1-create-an-application"></a>Etapa 1: criar um aplicativo

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a>Entrar no Microsoft Graph Explorer (recomendado), no Postman ou em qualquer outro cliente de API que você usa

1. Iniciar [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
2. Selecione **entrar com a Microsoft** e entre usando um administrador global do Azure ad ou credenciais de administrador de aplicativos.
3. Após entrar com êxito, você verá os detalhes da conta de usuário no painel esquerdo.

### <a name="create-an-application"></a>Criar um aplicativo

Para configurar o proxy de aplicativo para um aplicativo usando a API, você cria um aplicativo, adiciona uma entidade de serviço ao aplicativo e, em seguida, atualiza a propriedade **onPremisesPublishing** do aplicativo para definir as configurações de proxy de aplicativo. Ao criar o aplicativo, defina o **signInAudience** do aplicativo como "AzureADMyOrg".

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_application"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applications
Content-type: application/json

{
  "displayName": "Contoso IWA App",
  "signInAudience":"AzureADMyOrg"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "deletedDateTime": null,
  "addIns": [],
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "identifierUris": [],
  "createdDateTime": "2020-08-11T21:07:47.5919755Z",
  "description": null,
  "displayName": "Contoso IWA App",
  "isAuthorizationServiceEnabled": false,
  "isDeviceOnlyAuthSupported": null,
  "isFallbackPublicClient": null,
  "groupMembershipClaims": null,
  "notes": null,
  "optionalClaims": null,
  "orgRestrictions": [],
  "publisherDomain": "f128.info",
  "signInAudience": "AzureADandPersonalMicrosoftAccount",
  "tags": [],
  "tokenEncryptionKeyId": null,
  "uniqueName": null,
  "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
  },
}
```

### <a name="retrieve-the-application-object-id-and-appid"></a>Recuperar a ID de objeto de aplicativo e appId
Use a resposta da chamada anterior para recuperar e salvar a ID do objeto de aplicativo e a ID do aplicativo.
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a>Criar um servicePrincipalName para o aplicativo e adicionar marcas necessárias
Use a **AppID** para criar uma entidade de serviço para o aplicativo. Em seguida, adicione as marcas necessárias para configurar o proxy de aplicativo para um aplicativo.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_servicePrincipal"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/serviceprincipals
Content-type: appplication/json

{
  "appId":"d7fbfe28-c60e-46d2-8335-841923950d3b",
  "tags": [
    "WindowsAzureActiveDirectoryIntegratedApp",
    "WindowsAzureActiveDirectoryOnPremApp"
  ]
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals/$entity",
  "id": "a8cac399-cde5-4516-a674-819503c61313",
  "deletedDateTime": null,
  "accountEnabled": true,
  "alternativeNames": [],
  "createdDateTime": null,
  "deviceManagementAppType": null,
  "appDescription": null,
  "appDisplayName": "Contoso IWA App",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "appOwnerOrganizationId": "7918d4b5-0442-4a97-be2d-36f9f9962ece",
  "appRoleAssignmentRequired": false,
  "description": null,
  "displayName": "vtestapi2",
  "errorUrl": null,
  "homepage": null,
  "isAuthorizationServiceEnabled": false,
  "loginUrl": null,
  "logoutUrl": null,
  "notes": null,
  "notificationEmailAddresses": [],
  "preferredSingleSignOnMode": null,
  "preferredTokenSigningKeyEndDateTime": null,
  "preferredTokenSigningKeyThumbprint": null,
  "publisherName": "f/128 Photography",
  "replyUrls": [],
  "samlMetadataUrl": null,
  "samlSingleSignOnSettings": null,
  "servicePrincipalNames": [
      "b92b92d4-3874-46a5-b715-a00ea01cff93"
  ],
  "servicePrincipalType": "Application",
}
```

## <a name="step-2-configure-application-proxy-properties"></a>Etapa 2: configurar as propriedades do proxy de aplicativo

### <a name="set-the-onpremisespublishing-configuration"></a>Definir a configuração do onPremisesPublishing

Use a ID de objeto de aplicativo da etapa anterior para configurar o proxy de aplicativo para o aplicativo e atualizar a propriedade **onPremisesPublishing** para a configuração desejada. Neste exemplo, você está usando um aplicativo com a URL interna: `https://contosoiwaapp.com` e usando o domínio padrão para a URL externa: `https://contosoiwaapp-contoso.msappproxy.net` . 

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
    "onPremisesPublishing": {
        "externalAuthenticationType": "aadPreAuthentication",
        "internalUrl": "https://contosoiwaapp.com",
        "externalUrl": "https://contosoiwaapp-contoso.msappproxy.net"
    }
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a>Concluir a configuração do aplicativo
Atualize as propriedades **redirectUri**, **identifierUri**e **HOMEPAGEURL** do aplicativo para a ur externa configurada na propriedade **onPremisesPublishing** . Em seguida, atualize o [implicitGrantSettings](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) para o `true` **EnabledTokenIssuance** e `false` para o **enabledAccessTokenIssuance**.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
  "identifierUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
  "web": {
    "redirectUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
    "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net",
    "implicitGrantSettings": {
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": false
    }
  }
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a>Etapa 3: atribuir o grupo de conectores ao aplicativo

### <a name="get-connectors"></a>Obter conectores

Liste os conectores e use a resposta para recuperar e salvar a ID de objeto do conector. A ID do objeto Connector será usada para atribuir o conector a um grupo de conectores.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectors",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectors",
    "value": [
        {
            "id": "d2b1e8e8-8511-49d6-a4ba-323cb083fbb0",
            "machineName": "connectorA.redmond.contoso.com"",
            "externalIp": "131.137.147.164",
            "status": "active"
        },
        {
            "id": "f2cab422-a1c8-4d70-a47e-2cb297a2e051",
            "machineName": "connectorB.contoso.com"",
            "externalIp": "68.0.191.210",
            "status": "active"
        },
        {
            "id": "8555cc3c-5c8b-48a8-a8b2-5e97c32ef907",
            "machineName": "connectorC.contoso.com",
            "externalIp": "40.78.66.161",
            "status": "active"
        }
    ]
}
```

### <a name="create-a-connectorgroup"></a>Criar um um dos conectores
Para este exemplo, um novo grupo de conectores é criado com o nome "grupo de conectores de demonstração do IWA" que é usado para o aplicativo. Você também pode ignorar esta etapa se o seu conector já estiver atribuído ao conector apropriado. Recupere e salve a ID de objeto do The Connector para usar na próxima etapa.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups

Content-type: application/json
{
   "name": "IWA Demo Connector Group"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 201
Content-type: connectorGroup/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectorGroups/$entity",
    "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
    "name": "IWA Demo Connector Group",
    "connectorGroupType": "applicationProxy",
    "isDefault": false
}
```

### <a name="assign-a-connector-to-the-connectorgroup"></a>Atribuir um conector ao conector

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/8555cc3c-5c8b-48a8-a8b2-5e97c32ef907/memberOf/$ref

Content-type: application/json
{
  "@odata.id":"https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a>Atribuir o aplicativo ao conector

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
PUT https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref
Content-type: application/json

{
"@odata.id":"https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a>Etapa 4: configurar o logon único
Este aplicativo usa a autenticação integrada do Windows (IWA). Para configurar o IWA, defina as propriedades de logon único no tipo de recurso [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) .

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
   "onPremisesPublishing": {
      "singleSignOnSettings": {
         "kerberosSignOnSettings": {
            "kerberosServicePrincipalName": "HTTP/iwademo.contoso.com",
        "kerberosSignOnMappingAttributeType": "userPrincipalName"
         },
         "singleSignOnMode": "onPremisesKerberos"
      }
   }
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a>Etapa 5. Atribuir usuários
### <a name="retrieve-approle-for-the-applicaiton"></a>Recuperar appRole para o aplicativo

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('a8cac399-cde5-4516-a674-819503c61313')/appRoles",
    "value": [
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "b9632174-c057-4f7e-951b-be3adc52bfe6",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        }
    ]
}
```

Use a resposta da chamada anterior para recuperar e salvar a ID de appRole a ser usada para a próxima etapa.
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a>Atribuir usuários e grupos ao aplicativo

Use as propriedades a seguir para atribuir um usuário ao aplicativo.

| Propriedade  | Descrição |ID  |
|---------|---------|---------|
| principalId | ID de usuário do usuário que será atribuído ao aplicativo | 2fe96d23-5dc6-4f35-8222-0426a8c115c8 |
| principalType | Tipo de usuário | Usuário |
| appRoleId |  A ID de função de aplicativo da função de aplicativo padrão do aplicativo | 18d14569-c3bd-439b-9a66-3a2aee01d14f |
| resourceId | A ID de servicePrincipalName do aplicativo | a8cac399-cde5-4516-a674-819503c61313 |

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"a8cac399-cde5-4516-a674-819503c61313"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
    "id": "I23pL8ZdNU-CIgQmqMEVyLJ0E6fx0ixEo92az8MnhtU",
    "creationTimestamp": "2020-06-09T00:06:07.5129268Z",
    "appRoleId": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
    "principalDisplayName": "Jean Green",
    "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
    "principalType": "User",
    "resourceDisplayName": "Contoso IWA App",
    "resourceId": "a8cac399-cde5-4516-a674-819503c61313"
}
```

Para saber mais, confira o tipo de recurso [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta).


## <a name="additional-steps"></a>Etapas adicionais
- [Configuração automatizada usando exemplos do PowerShell para o proxy de aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [Automação da configuração do aplicativo de SSO baseado em SAML com o Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
