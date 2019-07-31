---
title: tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão de OAuth 2,0 e funções de aplicativo no recurso especificado que um aplicativo exige acesso. Os escopos de permissão OAuth 2,0 especificados podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** ) ao chamar um aplicativo de recurso. A propriedade **requiredResourceAccess** da entidade Application é uma coleção de **ReqiredResourceAccess**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6c7fec2027e5e987c66f868cc4a69555141bdbf9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965413"
---
# <a name="requiredresourceaccess-resource-type"></a>tipo de recurso requiredResourceAccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|resourceAccess|Coleção [ResourceAccess](resourceaccess.md)|A lista de escopos de permissão OAuth 2.0 e funções de aplicativo que o aplicativo requer do recurso especificado.|
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
