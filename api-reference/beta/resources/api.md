---
title: tipo de recurso da API
description: Especifica as configurações para um aplicativo Web API.
ms.openlocfilehash: b5b07ccb5a66027f9eb755754842f6e2e2ae708e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035462"
---
# <a name="api-resource-type"></a>tipo de recurso da API

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Especifica as configurações para um aplicativo Web API.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|requestedAccessTokenVersion|Int32| Especifica a versão de token de acesso aceito para o recurso de API atual. Valores possíveis são 1 ou 2.  |
|oauth2PermissionScopes|coleção [permissionScope](permissionscope.md)| A coleção de escopos de permissão OAuth 2.0 que a web application API (recurso) expõe para os aplicativos cliente. Estes escopos de permissão podem ser concedidos aos aplicativos de cliente durante o consentimento. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->