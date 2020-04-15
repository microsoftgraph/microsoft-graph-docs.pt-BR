---
title: Tipo de recurso emailAddress
description: O nome e o endereço de email de um destinatário da mensagem ou contato.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0fb557e35248dbc1521d1b494c831146b4e30da8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463737"
---
# <a name="emailaddress-resource-type"></a>Tipo de recurso emailAddress

Namespace: microsoft.graph

O nome e o endereço de email de um destinatário da mensagem ou contato.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|Cadeia de caracteres|O endereço de email da pessoa ou entidade.|
|nome|String|O nome de exibição da pessoa ou entidade.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
