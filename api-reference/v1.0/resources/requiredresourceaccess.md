---
title: Tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão OAuth 2.0 e funções de aplicativo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ea14ac7d38dd44f16c548f5501e17c7e244c5214
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055868"
---
# <a name="requiredresourceaccess-resource-type"></a>Tipo de recurso requiredResourceAccess

Namespace: microsoft.graph

Especifica o conjunto de escopos de permissão OAuth 2.0 e funções de aplicativo sob o recurso especificado ao que um aplicativo requer acesso. Os escopos de permissão OAuth 2.0 especificados podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess)** ao chamar um aplicativo de recurso. A **propriedade requiredResourceAccess** da entidade [application](application.md) é uma coleção de **ReqiredResourceAccess**.


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
|resourceAccess|[coleção resourceAccess](resourceaccess.md)|A lista de escopos de permissão OAuth2.0 e funções de aplicativo que o aplicativo exige do recurso especificado.|
|resourceAppId|String|O identificador exclusivo do recurso ao que o aplicativo requer acesso.  Isso deve ser igual ao **appId** declarado no aplicativo de recurso de destino.|

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

