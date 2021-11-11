---
title: Usar o Microsoft Graph para configurar permissões necessárias do Azure AD Graph para um registro de aplicativo
description: Use o Microsoft Graph para configurar permissões necessárias do Azure AD Graph para um registro de aplicativo.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 25fac773056238bde7c50158eb09daf3f5080552
ms.sourcegitcommit: 6b5bee1a1cea92c1f3d6439110c4916eb8b249a5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/11/2021
ms.locfileid: "60908579"
---
# <a name="use-microsoft-graph-to-configure-required-azure-ad-graph-permissions-for-an-app-registration"></a>Usar o Microsoft Graph para configurar permissões necessárias do Azure AD Graph para um registro de aplicativo

Azure Active Directory (Azure AD) Graph está preterido e será retirado em 30 de junho de 2022. Como parte desse caminho de depreciação, a adição de permissões do Azure AD Graph permissões necessárias para um registro de aplicativo por meio do portal do Azure agora está desabilitada. Recomendamos que você siga a lista de verificação planejamento [de](migrate-azure-ad-graph-planning-checklist.md) migração de aplicativos para ajudá-lo a fazer a transição de seus aplicativos para a [API Graph](/graph/overview) Microsoft.

No entanto, talvez você ainda precise adicionar mais permissões do Azure AD Graph seu aplicativo. Este artigo fornece orientações sobre como usar o Microsoft Graph para configurar permissões necessárias para o Azure AD Graph para o registro do aplicativo.

> [!CAUTION]
> Qualquer aplicativo usando o Azure AD Graph ainda irá parar de funcionar após 30 de junho de 2022. Para obter mais informações, [consulte Migrate Azure AD Graph aplicativos para o Microsoft Graph](migrate-azure-ad-graph-overview.md).

## <a name="option-1-use-the-microsoft-graph-api"></a>Opção 1: Usar a API Graph Microsoft

A API Graph [aplicativo](/graph/api/resources/application) da Microsoft inclui uma propriedade **requiredResourceAccess** que é uma coleção de objetos [requiredResourceAccess.](/graph/api/resources/requiredresourceaccess) Use essa propriedade para configurar permissões necessárias do Azure AD Graph conforme descrito nas etapas a seguir.

### <a name="prerequisites"></a>Pré-requisitos

Para concluir as etapas a seguir, você precisa dos seguintes recursos e privilégios:

+ Execute as solicitações HTTP em uma ferramenta de sua escolha, por exemplo, em seu aplicativo, [Graph Explorer](https://aka.ms/ge)ou Postman.
+ Execute as APIs como um usuário em uma função administrador global ou administrador de aplicativos ou como proprietário do registro do aplicativo de destino. Para obter mais informações sobre as ações suportadas por essas funções, consulte Funções integradas do [Azure AD](/azure/active-directory/roles/permissions-reference).
+ O aplicativo usado para fazer essas alterações deve ter a `Application.ReadWrite.All` permissão concedida.

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Etapa 1: Identificar as IDs de permissão para o Azure AD Graph permissões que seu aplicativo exige

Identifique as permissões do Azure AD Graph seu aplicativo, suas IDs de permissão e se elas são funções de aplicativo (permissões de aplicativo) ou permissões delegadas. Você pode recuperar as IDs de permissão de um registro de aplicativo existente que tenha a permissão configurada lendo sua propriedade **requiredResourceAccess** no **Manifesto** do aplicativo no portal do Azure ou por meio da API do Microsoft Graph. 

O Azure AD Graph **appId** global exclusivo do Azure é e é identificado pela propriedade `00000002-0000-0000-c000-000000000000` **resourceAppId** da propriedade **requiredResourceAccess.**

### <a name="request"></a>Solicitação

A solicitação a seguir recupera as IDs e tipos de permissão do Azure AD Graph de um aplicativo existente identificado **por id** `f7748341-825c-46e9-a111-5e3b56ae015b` .

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-get-serviceprincipal-azureadgraph"
}-->

```msgraph-interactive
https://graph.microsoft.com/v1.0/applications/f7748341-825c-46e9-a111-5e3b56ae015b?$select=requiredResourceAccess
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications(requiredResourceAccess)/$entity",
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

A partir dessa saída, é a ID de permissão da permissão delegada User.Read enquanto é a ID de permissão da função de aplicativo `311a71cc-e848-46a1-bdf8-97ff7156d8e6`  `3afa6a7d-9b1a-42eb-948e-1650a849e176` *Application.Read.All.*

### <a name="step-2-add-required-azure-ad-graph-permissions-to-your-app"></a>Etapa 2: Adicionar permissões necessárias do Azure AD Graph seu aplicativo

O exemplo a seguir chama a [API](/graph/api/application-update) do aplicativo Update para adicionar as permissões necessárias do Azure AD Graph a um registro de aplicativo identificado pela ID do objeto `581088ba-83c5-4975-b8af-11d2d7a76e98` . Na Etapa 1, essas permissões eram *User.Read* e *Application.Read.All,* respectivamente.

> [!IMPORTANT]
> Para atualizar **a propriedade requiredResourceAccess,** você deve passar as permissões existentes e novas. Passar apenas novas permissões substitui e remove as permissões existentes.

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

### <a name="step-3-verify-that-the-required-azure-ad-graph-permissions-were-added-to-your-app"></a>Etapa 3: Verifique se as permissões necessárias do Azure AD Graph foram adicionadas ao seu aplicativo

Verifique se o registro do aplicativo tem as permissões de API necessárias adicionadas na Etapa 2 usando a API do Microsoft Graph ou verificando a página Registros de aplicativo **no** portal do Azure.

#### <a name="use-the-microsoft-graph-get-applicationid-api"></a>Usar a API GET /application/{id} da Microsoft Graph microsoft

A solicitação a seguir recupera **as propriedades id** **e requiredResourceAccess** do aplicativo identificado pela **id** do objeto `581088ba-83c5-4975-b8af-11d2d7a76e98` .

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98?$select=id,requiredResourceAccess
```

>**Observação:** Embora você tenha configurado as permissões que o aplicativo exige, essas permissões não foram concedidas. Muitas permissões exigem consentimento do administrador antes que possam ser usadas para acessar dados organizacionais.

## <a name="option-2-use-microsoft-graph-powershell"></a>Opção 2: Usar o Microsoft Graph PowerShell

O cmdlet [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true) no Microsoft Graph PowerShell inclui um parâmetro **RequiredResourceAccess** que é uma coleção de **objetos IMicrosoftGraphRequiredResourceAccess.** Use este parâmetro para configurar as permissões necessárias do Azure AD Graph conforme descrito nas etapas a seguir.

### <a name="prerequisites"></a>Pré-requisitos

Para concluir as etapas a seguir, os seguintes privilégios são necessários:

+ Uma sessão autenticada do PowerShell (por exemplo, usando `Connect-MgGraph` ).
+ O Microsoft Graph PowerShell deve ter a `Application.ReadWrite.All` permissão concedida.
+ O usuário inscreveu deve ter as funções de diretório Administrador Global ou Administrador de Aplicativos do Azure AD ou ser proprietário do registro do aplicativo de destino. Para obter mais informações sobre as ações suportadas por essas funções, consulte Funções integradas do [Azure AD](/azure/active-directory/roles/permissions-reference).

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Etapa 1: Identificar as IDs de permissão para o Azure AD Graph permissões que seu aplicativo exige

Identifique as permissões do Azure AD Graph seu aplicativo, suas IDs de permissão e se elas são funções de aplicativo (permissões de aplicativo) ou permissões delegadas. Você pode recuperar as IDs de permissão de um registro de aplicativo existente que tenha a permissão configurada lendo sua propriedade **RequiredResourceAccess** no **Manifesto** do aplicativo no portal do Azure ou por meio de um script do PowerShell.

### <a name="request"></a>Solicitação

Crie um novo script do PowerShell chamado **fetchPermissions.ps1** adicionar o código a seguir. Este código recupera as IDs e tipos de permissão do Azure AD Graph de um registro de aplicativo existente identificado pela ID do objeto `f7748341-825c-46e9-a111-5e3b56ae015b` . Substitua pela ID do objeto do aplicativo `f7748341-825c-46e9-a111-5e3b56ae015b` de origem.

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All" 

## Replace f7748341-825c-46e9-a111-5e3b56ae015b with the object ID of the existing app registration; then read and output the permission IDs and their types
$sourceAppId= 'f7748341-825c-46e9-a111-5e3b56ae015b' 
$sourceApp = Get-MgApplication -ApplicationId $sourceAppId 
$sourceApp.RequiredResourceAccess.ResourceAccess
```

Execute o script usando o comando a seguir
```powershell
.\fetchPermissions.ps1
```

### <a name="response"></a>Resposta

A seguir, um exemplo de saída.

```powershell
Id                                   Type
--                                   ----
311a71cc-e848-46a1-bdf8-97ff7156d8e6 Scope
3afa6a7d-9b1a-42eb-948e-1650a849e176 Role
```

A partir dessa saída, é a ID de permissão da permissão delegada User.Read enquanto é a ID de permissão da função de aplicativo `311a71cc-e848-46a1-bdf8-97ff7156d8e6`  `3afa6a7d-9b1a-42eb-948e-1650a849e176` *Application.Read.All.*

### <a name="step-2-add-azure-ad-graph-permissions-to-your-app"></a>Etapa 2: Adicionar permissões do Azure AD Graph seu aplicativo

Crie um novo script do PowerShell chamado **updatePermissions.ps1** adicionar o código a seguir. Este código adiciona as permissões necessárias do Azure AD Graph a um registro de aplicativo identificado pela ID do objeto `581088ba-83c5-4975-b8af-11d2d7a76e98` . Na Etapa 1, essas permissões eram *User.Read* e *Application.Read.All,* respectivamente.

> [!IMPORTANT]
> Para atualizar **a propriedade RequiredResourceAccess,** você deve passar as permissões existentes e novas. Passar apenas novas permissões substitui e remove as permissões existentes.

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
