---
title: Configurar permissões necessárias do Azure AD Graph para um registro de aplicativo
description: Configure permissões necessárias do Azure AD Graph para um registro de aplicativo.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: fa74def34e93bed88513e564931a5b6557ed1bc8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334986"
---
# <a name="configure-required-azure-ad-graph-permissions-for-an-app-registration"></a>Configurar permissões necessárias do Azure AD Graph para um registro de aplicativo

Azure Active Directory (Azure AD) Graph está preterido e será retirado em um futuro próximo. Como parte desse caminho de depreciação, a adição de permissões do Azure AD Graph a um registro de aplicativo por meio do portal do Azure agora está desabilitada. Recomendamos que você siga a lista de verificação planejamento [de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md) para ajudá-lo a fazer a transição de seus aplicativos para [a API Graph](/graph/overview) Microsoft.

No entanto, seu aplicativo ainda pode exigir temporariamente permissões do Azure AD Graph acessar recursos. Este artigo descreve os quatro métodos a seguir para configurar permissões necessárias do Azure AD Graph para o registro do aplicativo:

1. [Usar o portal do Azure para encontrar as APIs que sua organização usa](#option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses)
1. [Atualizar o manifesto do aplicativo no portal do Azure](#option-2-update-the-application-manifest-on-the-azure-portal)
1. [Usar a API do Microsoft Graph](#option-3-use-the-microsoft-graph-api)
1. [Usar o Microsoft Graph PowerShell SDK](#option-4-use-the-microsoft-graph-powershell-sdk)

> [!CAUTION]
> Todos os aplicativos que usam o Azure AD Graph continuarão funcionando depois que o Azure AD Graph API. Para obter mais informações, [consulte Migrate Azure AD Graph aplicativos para o Microsoft Graph](migrate-azure-ad-graph-overview.md).

## <a name="option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses"></a>Opção 1: Usar o portal do Azure para encontrar as APIs que sua organização usa

1. Entre no [portal do Azure](https://portal.azure.com) como administrador global ou administrador de aplicativos.
1. Pesquise e **selecione Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativos**, na guia  Todos os aplicativos, selecione o aplicativo para o qual você deseja adicionar permissões do Azure AD Graph. Isso abre o painel Visão geral **do registro do** aplicativo.
1. No painel esquerdo da janela, no **grupo de menu** Gerenciar, selecione **Permissões de API**. Isso revela as **permissões configuradas para** o registro do aplicativo. Selecione **Adicionar uma permissão**.
1. Na janela **Solicitação de** permissões de API que é revelada, alterne para **as APIs que minha organização usa** guia e pesquisa ou `Windows Azure Active Directory` `00000002-0000-0000-c000-000000000000`. Selecione na lista filtrada para revelar a janela **Azure Active Directory Graph** permissões.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AzureADGraphPermissionsAPI.png" alt-text="A API de Graph do Azure AD é identificada pelo Windows Azure Active Directory e clientID 00000002-0000-0000-c000-00000000000000000." border="true":::

1. Selecione a **guia Permissões delegadas** ou **permissões de aplicativo para** escolher entre permissões delegadas e de aplicativo, respectivamente. Selecione **Adicionar permissões para** adicionar a permissão ao registro do aplicativo.
1. Depois de adicionar as permissões de que você precisa, na  janela Permissões Configuradas, selecione Conceder  consentimento ao administrador para conceder o Azure AD Graph permissões ao registro do aplicativo.

## <a name="option-2-update-the-application-manifest-on-the-azure-portal"></a>Opção 2: Atualizar o manifesto do aplicativo no portal do Azure

1. Entre no [portal do Azure](https://portal.azure.com) como administrador global ou administrador de aplicativos.
1. Pesquise e **selecione Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativos**, na guia  Todos os aplicativos, selecione o aplicativo para o qual você deseja adicionar permissões do Azure AD Graph. Isso abre o painel Visão geral **do registro do** aplicativo.
1. No painel esquerdo da janela, no grupo de menu **Gerenciar** , selecione **Manifesto**. Isso abre um editor que permite editar diretamente os atributos do objeto de registro do aplicativo.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppRegistrationManifest.png" alt-text="Um arquivo de manifesto de registro de aplicativo permite que você edite os atributos do aplicativo." border="true":::

1. Edite cuidadosamente **a propriedade requiredResourceAccess** no arquivo de manifesto do aplicativo para adicionar os seguintes detalhes:
    >**Observação:** Você pode editar o manifesto do aplicativo no portal do Azure ou selecionar **Baixar** para editar o manifesto localmente e, em  seguida, usar o Upload para reaplicar para seu aplicativo.
+ Adicione a **propriedade resourceAppId** e atribua o valor `00000002-0000-0000-c000-000000000000` que representa o Azure AD Graph
+ Adicione a **propriedade resourceAccess** e atribua as permissões necessárias.

    O trecho JSON a seguir mostra uma propriedade **requiredResourceAccess** com o Azure AD Graph como o recurso e atribuiu *user.Read* e *Application.Read.All* oauth2PermissionScope (permissão delegada) e appRole (permissão de aplicativo), respectivamente.    

    ```JSON
    "requiredResourceAccess": [
        {
            "resourceAppId": "00000002-0000-0000-c000-000000000000",
            "resourceAccess": [
                {
                    "id": "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
                    "type": "Scope"
                },
                {
                    "id": "3afa6a7d-9b1a-42eb-948e-1650a849e176",
                    "type": "Role"
                }
            ]
        }
    ],
    ```

7. Salve suas alterações.
8. Selecione **permissões de API** e nas permissões  configuradas para o registro do aplicativo, selecione Conceder  consentimento ao administrador para conceder ao Azure AD Graph permissões para o registro do aplicativo.

## <a name="option-3-use-the-microsoft-graph-api"></a>Opção 3: Usar a API Graph Microsoft

A API Graph [aplicativo](/graph/api/resources/application) da Microsoft inclui uma propriedade **requiredResourceAccess** que é uma coleção [de objetos requiredResourceAccess](/graph/api/resources/requiredresourceaccess). Use essa propriedade para configurar permissões necessárias do Azure AD Graph conforme descrito nas etapas a seguir.

### <a name="prerequisites"></a>Pré-requisitos

Para concluir as etapas a seguir, você precisa dos seguintes recursos e privilégios:

+ Execute as solicitações HTTP em uma ferramenta de sua escolha, por exemplo, em seu aplicativo, [Graph Explorer](https://aka.ms/ge) ou Postman.
+ Execute as APIs como um usuário em uma função administrador global ou administrador de aplicativos ou como proprietário do registro do aplicativo de destino. Para obter mais informações sobre as ações suportadas por essas funções, consulte Funções integradas do [Azure AD](/azure/active-directory/roles/permissions-reference).
+ O aplicativo usado para fazer essas alterações deve ter a permissão `Application.ReadWrite.All` concedida.

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Etapa 1: Identificar as IDs de permissão para o Azure AD Graph permissões que seu aplicativo exige

Identifique as permissões do Azure AD Graph seu aplicativo, suas IDs de permissão e se elas são funções de aplicativo (permissões de aplicativo) ou oauth2PermissionScopes (permissões delegadas).

O Azure AD Graph é identificado como um objeto servicePrincipal `00000002-0000-0000-c000-000000000000` com como seu appId `Windows Azure Active Directory` global exclusivo e como **seu displayName** e **appDisplayName**. Execute a seguinte solicitação para recuperar o objeto de entidade de serviço do Azure AD Graph.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-get-serviceprincipal-azureadgraph"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$filter=appId eq '00000002-0000-0000-c000-000000000000'
```

#### <a name="response"></a>Resposta

No objeto response, detalhes para permissões de aplicativo do Azure AD Graph são listados no objeto **appRoles** enquanto os detalhes para permissões delegadas são listados no **objeto oauth2PermissionScopes**.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals",
    "value": [
        {
            "id": "1804a6f8-e623-4520-8f40-ba1b0c11c42d",
            "accountEnabled": true,
            "appDisplayName": "Windows Azure Active Directory",
            "appDescription": null,
            "appId": "00000002-0000-0000-c000-000000000000",
            "appOwnerOrganizationId": "f8cdef31-a31e-4b4a-93e4-5f571e91255a",
            "appRoleAssignmentRequired": false,
            "displayName": "Windows Azure Active Directory",
            "servicePrincipalNames": [
                "https://graph.windows.net",
                "00000002-0000-0000-c000-000000000000/graph.microsoftazure.us",
                "00000002-0000-0000-c000-000000000000/graph.windows.net",
                "00000002-0000-0000-c000-000000000000/directory.windows.net",
                "00000002-0000-0000-c000-000000000000",
                "https://graph.windows.net/",
                "https://graph.microsoftazure.us"
            ],
            "servicePrincipalType": "Application",
            "signInAudience": "AzureADMultipleOrgs",
            "appRoles": [
                {
                    "allowedMemberTypes": [
                        "Application"
                    ],
                    "description": "Allows the app to read applications and service principals without a signed-in user",
                    "displayName": "Read all applications",
                    "id": "3afa6a7d-9b1a-42eb-948e-1650a849e176",
                    "isEnabled": true,
                    "origin": "Application",
                    "value": "Application.Read.All"
                }
            ],
            "oauth2PermissionScopes": [
                {
                    "adminConsentDescription": "Allows users to sign in to the app, and allows the app to read the profile of signed-in users. It also allow the app to read basic company information of signed-in users.",
                    "adminConsentDisplayName": "Sign in and read user profile",
                    "id": "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
                    "isEnabled": true,
                    "type": "User",
                    "userConsentDescription": "Allows you to sign in to the app with your work account and let the app read your profile. It also allows the app to read basic company information.",
                    "userConsentDisplayName": "Sign you in and read your profile",
                    "value": "User.Read"
                }
            ]
        }
    ]
}
```

Na saída truncada acima, `311a71cc-e848-46a1-bdf8-97ff7156d8e6` está a ID de permissão para a permissão delegada *User.Read* `3afa6a7d-9b1a-42eb-948e-1650a849e176` enquanto é a ID de permissão para a permissão do aplicativo *Application.Read.All* .

### <a name="step-2-add-required-azure-ad-graph-permissions-to-your-app"></a>Etapa 2: Adicionar permissões necessárias do Azure AD Graph ao seu aplicativo

O exemplo a seguir chama [a API do](/graph/api/application-update) aplicativo Update para adicionar as permissões necessárias do Azure AD Graph a um registro de aplicativo identificado pela ID do objeto `581088ba-83c5-4975-b8af-11d2d7a76e98`. Na Etapa 1, essas permissões eram *User.Read* e *Application.Read.All* , respectivamente.

> [!IMPORTANT]
> Para atualizar **a propriedade requiredResourceAccess** , você deve passar as permissões existentes e novas. Passar apenas novas permissões substitui e remove as permissões existentes.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-update-application"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98
Content-Type: application/json

{
    "requiredResourceAccess": [
        {
            "resourceAppId": "00000002-0000-0000-c000-000000000000",
            "resourceAccess": [
                {
                    "id": "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
                    "type": "Scope"
                },
                {
                    "id": "3afa6a7d-9b1a-42eb-948e-1650a849e176",
                    "type": "Role"
                }
            ]
        }
    ]
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="step-3-verify-that-the-required-azure-ad-graph-permissions-were-added-to-your-app"></a>Etapa 3: Verificar se as permissões necessárias do Azure AD Graph foram adicionadas ao seu aplicativo

Verifique se o registro do aplicativo tem as permissões de API do Azure AD Graph que você adicionou na Etapa 2 usando a API do Microsoft Graph ou verificando a página Registros de aplicativo **no** portal do Azure.

#### <a name="use-the-microsoft-graph-get-applicationid-api"></a>Usar a API GET /application/{id} da Microsoft Graph

A solicitação a seguir recupera **as propriedades id** **e requiredResourceAccess** do aplicativo identificado pela **id do objeto** `581088ba-83c5-4975-b8af-11d2d7a76e98`.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98?$select=id,requiredResourceAccess
```

>**Observação:** Embora você tenha configurado as permissões que o aplicativo exige, essas permissões não foram concedidas. Muitas permissões exigem consentimento do administrador antes que possam ser usadas para acessar dados organizacionais.

## <a name="option-4-use-the-microsoft-graph-powershell-sdk"></a>Opção 4: Usar o Microsoft Graph PowerShell SDK

O cmdlet [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true) no Microsoft Graph PowerShell SDK inclui um parâmetro **RequiredResourceAccess** que é uma coleção de **objetos IMicrosoftGraphRequiredResourceAccess**. Use este parâmetro para configurar as permissões necessárias do Azure AD Graph conforme descrito nas etapas a seguir.

### <a name="prerequisites"></a>Pré-requisitos

Para concluir as etapas a seguir, os seguintes privilégios são necessários:

+ Uma sessão autenticada do PowerShell (por exemplo, usando `Connect-MgGraph`).
+ O Microsoft Graph PowerShell deve ter a `Application.ReadWrite.All` permissão concedida.
+ O usuário inscreveu deve ter as funções de diretório Administrador Global ou Administrador de Aplicativos do Azure AD ou ser proprietário do registro do aplicativo de destino. Para obter mais informações sobre as ações suportadas por essas funções, consulte Funções integradas do [Azure AD](/azure/active-directory/roles/permissions-reference).

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Etapa 1: Identificar as IDs de permissão para o Azure AD Graph permissões que seu aplicativo exige

Identifique as permissões do Azure AD Graph seu aplicativo, suas IDs de permissão e se são funções de aplicativo (permissões de aplicativo) ou permissões delegadas.

O Azure AD Graph é identificado como um objeto ServicePrincipal `00000002-0000-0000-c000-000000000000` com como seu AppId `Windows Azure Active Directory` global exclusivo e como **DisplayName** e **AppDisplayName**. Execute a seguinte solicitação para recuperar o objeto ServicePrincipal para o Azure AD Graph.

#### <a name="request"></a>Solicitação

Crie um novo script do PowerShell chamado **fetchPermissions.ps1** e adicione o código a seguir. Este código recupera as IDs e tipos de permissão do Azure AD Graph. A saída exibe e formatará a saída dos **objetos AppRoles** e **Oauth2PermissionScopes** .

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All"

# Retrieve the service principal details for Azure AD Graph API.
$AADGraph = Get-MgServicePrincipal -Filter "appId eq '00000002-0000-0000-c000-000000000000'"

# Format output of the request above and display AppRoles (application permissions) and oauth2PermissionScopes (delegated permissions)
Echo "Azure AD Graph service principal object and its supported permissions:"
Echo "Application permissions:"
$AADGraph.AppRoles | Format-List
Echo "Delegated permissions:"
$AADGraph.Oauth2PermissionScopes | Format-List
```

Execute o script usando o comando a seguir
```powershell
.\fetchPermissions.ps1
```

#### <a name="response"></a>Resposta

A seguir, um exemplo de saída.

```powershell
Welcome To Microsoft Graph!
Azure AD Graph service principal object and its supported permissions:
Application permissions:


AllowedMemberTypes   : {Application}
Description          : Allows the app to read applications and service principals without a signed-in user
DisplayName          : Read all applications
Id                   : 3afa6a7d-9b1a-42eb-948e-1650a849e176
IsEnabled            : True
Origin               : Application
Value                : Application.Read.All
AdditionalProperties : {}

Delegated permissions:


AdminConsentDescription : Allows users to sign in to the app, and allows the app to read the profile of signed-in users. It also allow the app to read basic company information of signed-in users.
AdminConsentDisplayName : Sign in and read user profile
Id                      : 311a71cc-e848-46a1-bdf8-97ff7156d8e6
IsEnabled               : True
Origin                  :
Type                    : User
UserConsentDescription  : Allows you to sign in to the app with your work account and let the app read your profile. It also allows the app to read basic company information.
UserConsentDisplayName  : Sign you in and read your profile
Value                   : User.Read
AdditionalProperties    : {}
```

A partir dessa saída, `311a71cc-e848-46a1-bdf8-97ff7156d8e6` está a ID de permissão da permissão delegada *User.Read* `3afa6a7d-9b1a-42eb-948e-1650a849e176` enquanto é a ID de permissão da permissão *application.Read.All* .

### <a name="step-2-add-azure-ad-graph-permissions-to-your-app"></a>Etapa 2: Adicionar permissões do Azure AD Graph seu aplicativo

Crie um novo script do PowerShell chamado **updatePermissions.ps1** e adicione o código a seguir. Este código adiciona as permissões necessárias do Azure AD Graph a um registro de aplicativo identificado pela ID do objeto `581088ba-83c5-4975-b8af-11d2d7a76e98`. Na Etapa 1, essas permissões eram *User.Read* e *Application.Read.All* , respectivamente.

> [!IMPORTANT]
> Para atualizar **a propriedade RequiredResourceAccess** , você deve passar as permissões existentes e novas. Passar apenas novas permissões substitui e remove as permissões existentes.

#### <a name="request"></a>Solicitação

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All" 

## Replace 581088ba-83c5-4975-b8af-11d2d7a76e98 with the object ID of the app you wish to add new permissions to
$applicationId = '581088ba-83c5-4975-b8af-11d2d7a76e98' 

$app = Get-MgApplication -ApplicationId $applicationId

## Azure AD Graph's globally unique appId is 00000002-0000-0000-c000-000000000000 identified by the ResourceAppId
$aadAccess = $app.RequiredResourceAccess | Where-Object { $_.ResourceAppId -eq '00000002-0000-0000-c000-000000000000' } 

if($null -eq $aadAccess){ 
    $app.RequiredResourceAccess += @{  
        ResourceAppId = "00000002-0000-0000-c000-000000000000"; 
        ResourceAccess = @( 

                ## Replace the following with values of ID and type for all permissions - both new and existing permissions - you want to configure for the app
                @{ 
                    # User.Read delegated permission Sign in and read user profile 
                    id = "311a71cc-e848-46a1-bdf8-97ff7156d8e6";  
                    type = "Scope"; 
                }, 
                @{ 
                    # Application.Read.All app role (application permission) to view application data
                    id = "3afa6a7d-9b1a-42eb-948e-1650a849e176"; 
                    type = "Role"; 
                }
            ) 
     } 
} 

Update-MgApplication -ApplicationId $applicationId -RequiredResourceAccess $app.RequiredResourceAccess 
```

Execute o script usando o comando a seguir.
```powershell
.\updatePermissions.ps1
```

### <a name="response"></a>Resposta

A seguir, um exemplo de saída.

```powershell
Welcome To Microsoft Graph!
```

>**Observação:** Embora você tenha configurado as permissões que o aplicativo exige, essas permissões não foram concedidas. Muitas permissões exigem consentimento do administrador antes que possam ser usadas para acessar dados organizacionais.

## <a name="see-also"></a>Confira também

+ [API de aplicativo](/graph/api/resources/application)
+ [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true)
