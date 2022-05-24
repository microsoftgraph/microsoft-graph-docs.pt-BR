---
title: Atualizar configurações
description: Atualize uma ou mais configurações de nível de locatário SharePoint e OneDrive.
author: liamfernandez
ms.localizationpriority: medium
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 07abcd226649c175fe6906a3b15e14971d8e9cf7
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653598"
---
# <a name="update-settings"></a>Atualizar configurações
Namespace: microsoft.graph.tenantAdmin

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize uma ou mais configurações de nível [de](../resources/tenantadmin-settings.md) locatário para SharePoint e OneDrive.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|SharePointTenantSettings.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|SharePointTenantSettings.ReadWrite.All|

Ao chamar em nome de um usuário, o usuário precisa pertencer a uma das funções de administrador a seguir. Para saber mais sobre as funções de administrador, consulte [Sobre as funções de administrador no Centro de administração do Microsoft 365](/microsoft-365/admin/add-users/about-admin-roles):
* Administrador Global
* Administrador do SharePoint

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /admin/sharepoint/settings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]
A tabela a seguir mostra as propriedades que podem ser editadas para um [objeto de](../resources/tenantadmin-settings.md) configurações.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| allowedDomainGuidsForSyncApp                       | Coleção de GUIDs              | Coleção de GUIDs de domínio confiável para o Sincronização do OneDrive aplicativo.                                                                                                                                                  |
| deletedUserPersonalSiteRetentionPeriodInDays       | Int32                        | O número de dias para preservar os dados de um usuário excluído OneDrive.                                                                                                                                                   |
| excludedFileExtensionsForSyncApp                   | Coleção de cadeias de caracteres            | Coleção de extensões de arquivo não carregadas pelo Sincronização do OneDrive aplicativo.                                                                                                                                           |
| imageTaggingOption                                 | imageTaggingChoice           | Especifica a opção de marcação de imagem para o locatário. Os valores possíveis são: `disabled`, `basic`, `enhanced`.                                                                                                       |
| isCommentingOnSitePagesEnabled                     | Booliano                      | Indica se os comentários são permitidos em páginas de site modernas SharePoint.                                                                                                                                          |
| isFileActivityNotificationEnabled                  | Boolean                      | Indica se as notificações por push estão habilitadas para OneDrive eventos.                                                                                                                                               |
| isLoopEnabled                                      | Booliano                      | Indica se o Fluid Framework é permitido em SharePoint sites.                                                                                                                                                   |
| isMacSyncAppEnabled                                | Booliano                      | Indica se os arquivos podem ser sincronizados usando o aplicativo Sincronização do OneDrive para Mac.                                                                                                                                          |
| isResharingByExternalUsersEnabled                  | Booliano                      | Indica se os convidados têm permissão para compartilhar novamente arquivos, pastas e sites que eles não têm.                                                                                                                           |
| isSharePointMobileNotificationEnabled              | Booliano                      | Indica se as notificações por push móveis estão habilitadas para SharePoint.                                                                                                                                             |
| isSharePointNewsfeedEnabled                        | Booliano                      | Indica se o news feed é permitido nas páginas modernas do site SharePoint.                                                                                                                                   |
| isSiteCreationEnabled                              | Booliano                      | Indica se os usuários têm permissão para criar sites.                                                                                                                                                           |
| isSiteCreationUIEnabled                            | Boolean                      | Indica se os comandos da interface do usuário para criar sites são mostrados.                                                                                                                                                     |
| isSitePagesCreationEnabled                         | Booliano                      | Indica se a criação de novas páginas modernas é permitida SharePoint sites.                                                                                                                                         |
| isSitesStorageLimitAutomatic                       | Boolean                      | Indica se o espaço de armazenamento do site é gerenciado automaticamente ou se os limites de armazenamento específicos são definidos por site.                                                                                                       |
| isSyncButtonHiddenOnPersonalSite                   | Booliano                      | Indica se o botão de sincronização no OneDrive está oculto.                                                                                                                                                            |
| isUnmanagedSyncAppForTenantRestricted              | Boolean                      | Indica se os usuários têm permissão para sincronizar arquivos somente em computadores ingressados em domínios específicos.                                                                                                                           |
| personalSiteDefaultStorageLimitInMB                | Int64                        | O padrão OneDrive limite de armazenamento para todos os usuários novos e existentes que recebem uma licença qualificada. Medido em megabytes (MB).                                                                           |
| sharingAllowedDomainList                           | Coleção de cadeias de caracteres            | Coleção de domínios de email permitidos para compartilhamento fora da organização.                                                                                                                              |
| sharingBlockedDomainList                           | Coleção de cadeias de caracteres            | Coleção de domínios de email bloqueados para compartilhamento fora da organização.                                                                                                                              |
| sharingCapability                                  | sharingCapabilities          | Capacidade de compartilhamento para o locatário. Os valores possíveis são: `disabled`, `externalUserSharingOnly`, `externalUserAndGuestSharing`, `existingExternalUserSharingOnly`.                                                |
| sharingDomainRestrictionMode                       | sharingDomainRestrictionMode | Especifica o modo compartilhamento externo para os domínios. Os valores possíveis são: `none`, `allowList`, `blockList`.                                                                                                        |
| siteCreationDefaultManagedPath                     | Cadeia de caracteres                       | O valor do caminho gerenciado do site de equipe. Esse é o caminho no qual novos sites de equipe serão criados.                                                                                                          |
| siteCreationDefaultStorageLimitInMB                | Int32                        | A cota de armazenamento padrão para um novo site após a criação. Medido em megabytes (MB).                                                                                                                            |
| tenantDefaultTimezone                              | Cadeia de caracteres                       | O fuso horário padrão de um locatário para sites recém-criados.                                                                                                                                                      |




## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e um objeto [de configurações](../resources/tenantadmin-settings.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "update_tenant_settings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/sharepoint/settings
Content-Type: application/json
Content-length: 1323

{
    "deletedUserPersonalSiteRetentionPeriodInDays": 365,
    "excludedFileExtensionsForSyncApp": [".mp3"],
    "imageTaggingOption": "enhanced",
    "isSitesStorageLimitAutomatic": false,
    "isSyncButtonHiddenOnPersonalSite": false,
    "isUnmanagedSyncAppForTenantRestricted": false,
    "personalSiteDefaultStorageLimitInMB": 120000
}
```


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tenantAdmin.settings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.tenantAdmin.settings",
    "id": "e79403fa-abdf-af49-56c5-f7119d8b1948",
    "allowedDomainGuidsForSyncApp": [
        "bdd1ab9b-3fd0-4def-a761-ec8d7471732c", 
        "ad31vb6b-5zd0-7tyg-m231-kj8d6578432c"
    ],
    "availableManagedPathsForSiteCreation": [
        "/sites/",
        "/teams/"
    ],
    "deletedUserPersonalSiteRetentionPeriodInDays": 365,
    "excludedFileExtensionsForSyncApp": [
        ".mp3"
    ],
    "imageTaggingOption": "basic",
    "isCommentingOnSitePagesEnabled": true,
    "isFileActivityNotificationEnabled": true,
    "isLoopEnabled": true,
    "isMacSyncAppEnabled": false,
    "isResharingByExternalUsersEnabled": true,
    "isSharePointMobileNotificationEnabled": true,
    "isSharePointNewsfeedEnabled": true,
    "isSiteCreationEnabled": true,
    "isSiteCreationUIEnabled": true,
    "isSitePagesCreationEnabled": true,
    "isSitesStorageLimitAutomatic": false,
    "isSyncButtonHiddenOnPersonalSite": false,
    "isUnmanagedSyncAppForTenantRestricted": false,
    "personalSiteDefaultStorageLimitInMB": 120000,
    "sharingAllowedDomainList" : [
        "contoso.com",
        "fabrikam.com"
    ],
    "sharingBlockedDomainList" : [
        "contoso.com",
        "fabrikam.com"
    ],
    "sharingCapability": "externalUserAndGuestSharing",
    "sharingDomainRestrictionMode": "allowList",
    "siteCreationDefaultManagedPath": "/sites/",
    "siteCreationDefaultStorageLimitInMB": 808034,
    "tenantDefaultTimezone": "(UTC-05:00) Eastern Time (US and Canada)"
}
```
