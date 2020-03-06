---
title: tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão OAuth 2,0 e funções de aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 45b7e8d2598ca58ef4d78bb45c3b2a8f51955353
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533839"
---
# <a name="requiredresourceaccess-resource-type"></a>tipo de recurso requiredResourceAccess

Namespace: microsoft.graph

Especifica o conjunto de escopos de permissão de OAuth 2,0 e funções de aplicativo no recurso especificado que um aplicativo exige acesso. Os escopos de permissão OAuth 2,0 especificados podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** ) ao chamar um aplicativo de recurso. A propriedade **requiredResourceAccess** da entidade [Application](application.md) é uma coleção de **ReqiredResourceAccess**.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|resourceAccess|coleção [resourceAccess](resourceaccess.md)|A lista de escopos de permissão OAuth 2.0 e funções de aplicativo que o aplicativo requer do recurso especificado.|
|resourceAppId|String|O identificador exclusivo do recurso ao qual o aplicativo exige acesso.  Isso deve ser igual ao **AppID** declarado no aplicativo de recurso de destino.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
