---
title: Tipo de recurso emailAddress
description: O nome e o endereço de email de um destinatário da mensagem ou contato.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 111c2c3b2be02512c66b4786fa17151c749dfd49
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126818"
---
# <a name="emailaddress-resource-type"></a>Tipo de recurso emailAddress

Namespace: microsoft.graph

O nome e o endereço de email de um destinatário da mensagem ou contato.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|Cadeia de caracteres|O endereço de email da pessoa ou entidade.|
|nome|Cadeia de caracteres|O nome de exibição da pessoa ou entidade.|

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

