---
title: tipo de recurso de resourceAccess
description: Especifica um escopo de permissão do OAuth 2.0 ou uma função do aplicativo que requer um aplicativo. A propriedade **resourceAccess** do tipo requiredResourceAccess é uma coleção de **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: f5389915897c3aab8b8277a45b54042bc861b290
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862332"
---
# <a name="resourceaccess-resource-type"></a>tipo de recurso de resourceAccess

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Especifica um escopo de permissão do OAuth 2.0 ou uma função do aplicativo que requer um aplicativo. A propriedade **resourceAccess** do tipo [requiredResourceAccess](requiredresourceaccess.md) é uma coleção de **ResourceAccess**.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Guid|O identificador exclusivo para uma das instâncias [oAuth2Permission](oauth2permission.md) ou [appRole](approle.md) que expõe o aplicativo do recurso.|
|type|Cadeia de caracteres|Especifica se a propriedade **id** faz referência a um [oAuth2Permission](oauth2permission.md) ou um [appRole](approle.md). Valores possíveis são "escopo" ou "role".|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
