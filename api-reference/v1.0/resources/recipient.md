---
title: Tipo de recurso recipient
description: 'Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo. '
ms.localizationpriority: medium
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a484a49e582d2df904dde65572453836b9d2fc4a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078662"
---
# <a name="recipient-resource-type"></a>Tipo de recurso recipient

Namespace: microsoft.graph

Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|emailAddress|[EmailAddress](emailaddress.md)|O endereço de email do destinatário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

