---
title: Configurar as permissões necessárias Azure AD Graph para um registro de aplicativo
description: Antes Azure AD Graph for desativado, você pode usar essas opções para configurar as permissões necessárias para o registro do aplicativo.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 76b80177954f4045ad74343e0cc1df018ec71848
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577893"
---
# <a name="configure-required-azure-ad-graph-permissions-for-an-app-registration"></a>Configurar as permissões necessárias Azure AD Graph para um registro de aplicativo

O Graph do Azure Active Directory (Azure AD) foi preterido e será desativado em um futuro próximo. Como parte desse caminho de substituição, adicionar permissões Azure AD Graph a um registro de aplicativo por meio do portal do Azure agora está desabilitado. Recomendamos que você siga a lista de verificação de planejamento de [migração de](migrate-azure-ad-graph-planning-checklist.md) aplicativos para ajudá-lo a fazer a transição de seus aplicativos para a API [do Microsoft Graph](/graph/overview) .

No entanto, seu aplicativo ainda pode exigir temporariamente Azure AD do Graph para acessar recursos. Este artigo descreve os quatro métodos a seguir para configurar as permissões Azure AD Graph necessárias para o registro do aplicativo:

1. [Use o portal do Azure para localizar as APIs que sua organização usa](#option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses)
1. [Atualizar o manifesto do aplicativo no portal do Azure](#option-2-update-the-application-manifest-on-the-azure-portal)
1. [Usar a API do Microsoft Graph](#option-3-use-the-microsoft-graph-api)
1. [Usar o SDK do PowerShell do Microsoft Graph](#option-4-use-the-microsoft-graph-powershell-sdk)

> [!CAUTION]
> Qualquer aplicativo que usa Azure AD Graph ainda interromperá o funcionamento após a desativação Azure AD API do Graph serviço. Para obter mais informações, consulte [Migrar aplicativos Azure AD Graph para o Microsoft Graph](migrate-azure-ad-graph-overview.md).

## <a name="option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses"></a>Opção 1: Usar o portal do Azure para localizar as APIs que sua organização usa

1. Entre no [portal do Azure como administrador](https://portal.azure.com) global ou administrador de aplicativos.
1. Pesquise e selecione **o Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativo**, na guia Todos os aplicativos, selecione o aplicativo para o qual você deseja adicionar Azure AD do Graph. Isso abre o painel Visão geral **do registro de** aplicativo.
1. No painel esquerdo da janela, no **grupo de** menus Gerenciar, selecione **permissões de API**. Isso revela as **permissões configuradas para** o registro do aplicativo. Selecione **Adicionar uma permissão**.
1. Na janela **Solicitar permissões de API** que é revelada, alterne para as **APIs** que minha organização usa guia e pesquise `Windows Azure Active Directory` ou `00000002-0000-0000-c000-000000000000`. Selecione na lista filtrada para revelar a janela de permissões do **Azure Active Directory Graph** .

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AzureADGraphPermissionsAPI.png" alt-text="Azure AD API do Graph é identificado pelo Windows Azure Active Directory e clientID 00000002-0000-0000-c000-00000000000000." border="true":::

1. Selecione a **guia Permissões delegadas ou** **permissões de aplicativo para** escolher entre permissões delegadas e de aplicativo, respectivamente. Selecione **Adicionar permissões para** adicionar a permissão ao registro do aplicativo.
1. Depois de adicionar as permissões necessárias, na janela Permissões Configuradas, selecione Conceder consentimento do administrador  para conceder as permissões do Azure AD Graph ao registro do aplicativo.

## <a name="option-2-update-the-application-manifest-on-the-azure-portal"></a>Opção 2: atualizar o manifesto do aplicativo no portal do Azure

1. Entre no [portal do Azure como administrador](https://portal.azure.com) global ou administrador de aplicativos.
1. Pesquise e selecione **o Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativo**, na guia Todos os aplicativos, selecione o aplicativo para o qual você deseja adicionar Azure AD do Graph. Isso abre o painel Visão geral **do registro de** aplicativo.
1. No painel esquerdo da janela, no grupo **de menus** Gerenciar, selecione **Manifesto**. Isso abre um editor que permite editar diretamente os atributos do objeto de registro do aplicativo.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppRegistrationManifest.png" alt-text="Um arquivo de manifesto de registro de aplicativo permite que você edite os atributos do aplicativo." border="true":::

1. Edite cuidadosamente **a propriedade requiredResourceAccess** no arquivo de manifesto do aplicativo para adicionar os seguintes detalhes:
    >**Nota:** Você pode editar o manifesto do aplicativo no portal do Azure ou selecionar **Baixar** para editar o manifesto localmente e, em seguida, usar **Carregar** para reaplicar ao seu aplicativo.
+ Adicione a **propriedade resourceAppId** e atribua o valor que `00000002-0000-0000-c000-000000000000` representa Azure AD Graph
+ Adicione a **propriedade resourceAccess** e atribua as permissões necessárias.

    O snippet JSON a seguir mostra uma propriedade **requiredResourceAccess** com o Azure AD Graph como o recurso e atribuiu *User.Read* e *Application.Read.All* oauth2PermissionScope (permissão delegada) e appRole (permissão de aplicativo), respectivamente.    

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
8. Selecione **permissões de API** e, nas  permissões configuradas para o registro do aplicativo, selecione  Conceder consentimento do administrador para conceder as permissões do Azure AD Graph ao registro do aplicativo.

## <a name="option-3-use-the-microsoft-graph-api"></a>Opção 3: Usar o Microsoft API do Graph

A API de aplicativo [do](/graph/api/resources/application) Microsoft Graph inclui uma propriedade **requiredResourceAccess** que é uma coleção de objetos  [requiredResourceAccess](/graph/api/resources/requiredresourceaccess) . Use essa propriedade para configurar as permissões Azure AD graph necessárias, conforme descrito nas etapas a seguir.

### <a name="prerequisites"></a>Pré-requisitos

Para concluir as etapas a seguir, você precisa dos seguintes recursos e privilégios:

+ Execute as solicitações HTTP em uma ferramenta de sua escolha, por exemplo, em seu aplicativo, por meio do [Explorador do Graph](https://aka.ms/ge) ou do Postman.
+ Execute as APIs como um usuário em uma função de Administrador Global ou Administrador de Aplicativos ou como proprietário do registro de aplicativo de destino. Para obter mais informações sobre as ações compatíveis com essas funções, [Azure AD funções internas](/azure/active-directory/roles/permissions-reference).
+ O aplicativo usado para fazer essas alterações deve receber a `Application.ReadWrite.All` permissão.

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Etapa 1: identificar as IDs de permissão para as Azure AD do Graph que seu aplicativo requer

Identifique as Azure AD do Graph que seu aplicativo requer, suas IDs de permissão e se elas são funções de aplicativo (permissões de aplicativo) ou oauth2PermissionScopes (permissões delegadas).

Azure AD Graph é identificado como um objeto servicePrincipal `00000002-0000-0000-c000-000000000000` com sua appId `Windows Azure Active Directory` globalmente exclusiva e como **displayName** e **appDisplayName**. Execute a solicitação a seguir para recuperar o objeto de entidade de serviço para Azure AD Graph.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-get-serviceprincipal-azureadgraph"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$filter=appId eq '00000002-0000-0000-c000-000000000000'
```

#### <a name="response"></a>Resposta

No objeto de resposta, os detalhes para permissões de aplicativo Azure AD Graph são listados no objeto **appRoles**, enquanto os detalhes das permissões delegadas são listados no **objeto oauth2PermissionScopes**.

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

### <a name="step-2-add-required-azure-ad-graph-permissions-to-your-app"></a>Etapa 2: Adicionar as permissões Azure AD Graph necessárias ao seu aplicativo

O exemplo a seguir chama [a API do](/graph/api/application-update) aplicativo Update para adicionar as permissões Azure AD Graph necessárias a um registro de aplicativo identificado pela ID do objeto`581088ba-83c5-4975-b8af-11d2d7a76e98`. Na Etapa 1, essas permissões foram *User.Read* e *Application.Read.All* delegadas permissão e permissão de aplicativo, respectivamente.

> [!IMPORTANT]
> Para atualizar **a propriedade requiredResourceAccess** , você deve passar permissões novas e existentes. Passar apenas novas permissões substitui e remove as permissões existentes.

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

### <a name="step-3-verify-that-the-required-azure-ad-graph-permissions-were-added-to-your-app"></a>Etapa 3: Verificar se as permissões Azure AD graph necessárias foram adicionadas ao seu aplicativo

Verifique se o registro do aplicativo tem as permissões Azure AD API do Graph necessárias que você adicionou na Etapa 2 usando o Microsoft API do Graph ou verificando **a página Registros de aplicativo** no portal do Azure.

#### <a name="use-the-microsoft-graph-get-applicationid-api"></a>Usar a API GET /application/{id} do Microsoft Graph

A solicitação a seguir recupera as **propriedades id** e **requiredResourceAccess** do aplicativo identificado pela **ID do objeto**`581088ba-83c5-4975-b8af-11d2d7a76e98`.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98?$select=id,requiredResourceAccess
```

>**Nota:** Embora você tenha configurado as permissões que o aplicativo requer, essas permissões não foram concedidas. Muitas permissões exigem consentimento do administrador antes que possam ser usadas para acessar dados organizacionais.

## <a name="option-4-use-the-microsoft-graph-powershell-sdk"></a>Opção 4: Usar o SDK do PowerShell do Microsoft Graph

O cmdlet [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true) no SDK do PowerShell do Microsoft Graph inclui um parâmetro **RequiredResourceAccess** que é uma coleção de **objetos IMicrosoftGraphRequiredResourceAccess** . Use esse parâmetro para configurar as permissões Azure AD graph necessárias, conforme descrito nas etapas a seguir.

### <a name="prerequisites"></a>Pré-requisitos

Para concluir as seguintes etapas, os seguintes privilégios são necessários:

+ Uma sessão autenticada do PowerShell (por exemplo, usando `Connect-MgGraph`).
+ O PowerShell do Microsoft Graph deve receber a `Application.ReadWrite.All` permissão.
+ O usuário conectado deve receber as funções de diretório administrador global ou administrador de aplicativos Azure AD ou ser proprietário do registro do aplicativo de destino. Para obter mais informações sobre as ações compatíveis com essas funções, [Azure AD funções internas](/azure/active-directory/roles/permissions-reference).

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Etapa 1: identificar as IDs de permissão para as Azure AD do Graph que seu aplicativo requer

Identifique as Azure AD do Graph necessárias para seu aplicativo, suas IDs de permissão e se elas são funções de aplicativo (permissões de aplicativo) ou permissões delegadas.

Azure AD Graph é identificado como um objeto ServicePrincipal `00000002-0000-0000-c000-000000000000` com sua AppId `Windows Azure Active Directory` globalmente exclusiva e como **DisplayName** e **AppDisplayName**. Execute a solicitação a seguir para recuperar o objeto ServicePrincipal para Azure AD Graph.

#### <a name="request"></a>Solicitação

Crie um script do PowerShell chamado **fetchPermissions.ps1** e adicione o código a seguir. Esse código recupera Azure AD IDs e tipos de permissão do Graph. A saída exibe e formatada a saída dos objetos **AppRoles** e **Oauth2PermissionScopes** .

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

Nessa saída, é `311a71cc-e848-46a1-bdf8-97ff7156d8e6` a ID de permissão da permissão delegada *User.Read* `3afa6a7d-9b1a-42eb-948e-1650a849e176` enquanto é a ID de permissão da permissão do aplicativo *Application.Read.All* .

### <a name="step-2-add-azure-ad-graph-permissions-to-your-app"></a>Etapa 2: Adicionar Azure AD do Graph ao seu aplicativo

Crie um script do PowerShell chamado **updatePermissions.ps1** e adicione o código a seguir. Esse código adiciona as permissões necessárias Azure AD Graph a um registro de aplicativo identificado pela ID do objeto`581088ba-83c5-4975-b8af-11d2d7a76e98`. Na Etapa 1, essas permissões foram *User.Read* e *Application.Read.All* delegadas permissão e permissão de aplicativo, respectivamente.

> [!IMPORTANT]
> Para atualizar **a propriedade RequiredResourceAccess** , você deve passar permissões novas e existentes. Passar apenas novas permissões substitui e remove as permissões existentes.

#### <a name="request"></a>Solicitação

```powershell
## Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All" 

## Azure AD Graph's globally unique appId is 00000002-0000-0000-c000-000000000000 identified by the ResourceAppId
$graphResourceId = "00000002-0000-0000-c000-000000000000"

## Replace 581088ba-83c5-4975-b8af-11d2d7a76e98 with the object ID of the app you wish to add new permissions to
$applicationId = "581088ba-83c5-4975-b8af-11d2d7a76e98" 

## Define the new permissions to be added to the target app
$newResourceAccess = @{  
    ResourceAppId = $graphResourceId; 
    ResourceAccess = @( 

        ## Replace the following with values of ID and type for all permissions you want to configure for the app
        @{ 
            # User.Read scope (delegated permission) to sign-in and read user profile 
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

$app = Get-MgApplication -ApplicationId $applicationId

## Get the existing permissions of the application
$existingResourceAccess = $app.RequiredResourceAccess

## If the app has no existing permissions, or no existing permissions from our new permissions resource
if ( ([string]::IsNullOrEmpty($existingResourceAccess) ) -or ($existingResourceAccess | Where-Object { $_.ResourceAppId -eq $graphResourceId } -eq $null) ) {
    $existingResourceAccess += $newResourceAccess
    Update-MgApplication -ApplicationId $applicationId -RequiredResourceAccess $existingResourceAccess
}

## If the app already has existing permissions from our new permissions resource
else {
    $newResourceAccess.ResourceAccess += $existingResourceAccess.ResourceAccess
    Update-MgApplication -ApplicationId $applicationId -RequiredResourceAccess $newResourceAccess
}
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

>**Nota:** Embora você tenha configurado as permissões que o aplicativo requer, essas permissões não foram concedidas. Muitas permissões exigem consentimento do administrador antes que possam ser usadas para acessar dados organizacionais.

## <a name="see-also"></a>Confira também

+ [API do aplicativo](/graph/api/resources/application)
+ [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true)
