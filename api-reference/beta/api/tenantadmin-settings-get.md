---
title: Obter configurações
description: Obtenha as configurações no nível do locatário para SharePoint e OneDrive.
author: liamfernandez
ms.localizationpriority: medium
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 2111ff6b45149a133de0022d50dd92042c0c3d60
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653586"
---
# <a name="get-settings"></a>Obter configurações
Namespace: microsoft.graph.tenantAdmin

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as configurações no nível [do](../resources/tenantadmin-settings.md) locatário para SharePoint e OneDrive.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|SharePointTenantSettings.Read.All, SharePointTenantSettings.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|SharePointTenantSettings.Read.All, SharePointTenantSettings.ReadWrite.All|

Ao chamar em nome de um usuário, o usuário precisa pertencer a uma das funções de administrador a seguir. Para saber mais sobre as funções de administrador, consulte [Sobre as funções de administrador no Centro de administração do Microsoft 365](/microsoft-365/admin/add-users/about-admin-roles):
* Administrador global
* Leitor global
* Administrador do SharePoint

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/sharepoint/settings
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e [um objeto de configurações](../resources/tenantadmin-settings.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "get_settings"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/sharepoint/settings
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
    "value": {
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
        "deletedUserPersonalSiteRetentionPeriodInDays": 344,
        "excludedFileExtensionsForSyncApp": [
            ".md", 
            ".git"
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
        "isSitesStorageLimitAutomatic": true,
        "isSyncButtonHiddenOnPersonalSite": true,
        "isUnmanagedSyncAppForTenantRestricted": true,
        "personalSiteDefaultStorageLimitInMB": 113664,
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
}
```

