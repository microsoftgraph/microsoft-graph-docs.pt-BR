---
title: Tipo de recurso requiredResourceAccess
description: Especifica o conjunto de escopos de permissão OAuth 2.0 e funções de aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 24d4e48fb6a15fabb61552d1ee2f2d884f276e6a862706b290fb97c1a2a78096
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184491"
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
|resourceAppId|Cadeia de caracteres|O identificador exclusivo do recurso ao que o aplicativo requer acesso.  Isso deve ser igual ao **appId** declarado no aplicativo de recurso de destino.|

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

