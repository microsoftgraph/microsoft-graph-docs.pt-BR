---
title: Tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão do OAuth 2.0 e funções de aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 0ca072b679a7ec3b69c311d09aaf2000f4754f19
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133256"
---
# <a name="requiredresourceaccess-resource-type"></a>Tipo de recurso requiredResourceAccess

Namespace: microsoft.graph

Especifica o conjunto de escopos de permissão OAuth 2.0 e funções de aplicativo sob o recurso especificado que um aplicativo requer acesso. Os escopos de permissão OAuth 2.0 especificados podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess)** ao chamar um aplicativo de recurso. A **propriedade requiredResourceAccess** da entidade [do](application.md) aplicativo é uma coleção de **ReqiredResourceAccess**.


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
|resourceAccess|[Coleção resourceAccess](resourceaccess.md)|A lista de escopos de permissão OAuth2.0 e funções de aplicativo que o aplicativo requer do recurso especificado.|
|resourceAppId|String|O identificador exclusivo do recurso ao que o aplicativo exige acesso.  Isso deve ser igual à **appId** declarada no aplicativo de recurso de destino.|

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

