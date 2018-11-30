---
title: Tipo de recurso emailAddress
description: O nome e o endereço de email de um destinatário da mensagem ou contato.
ms.openlocfilehash: 962b2f36af9e292125edc3da8606cd532b8c2ec0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003763"
---
# <a name="emailaddress-resource-type"></a>Tipo de recurso emailAddress

O nome e o endereço de email de um destinatário da mensagem ou contato.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|Cadeia de caracteres|O endereço de email da pessoa ou entidade.|
|name|Cadeia de caracteres|O nome de exibição da pessoa ou entidade.|

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
