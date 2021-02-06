---
title: Tipo de recurso emailAddress
description: Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário da mensagem ou proprietário do calendário.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8f572058d50672a26b3930f90a7b0492f9aa1eca
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132556"
---
# <a name="emailaddress-resource-type"></a>Tipo de recurso emailAddress

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário da mensagem ou proprietário do calendário.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|Cadeia de caracteres|O endereço de email de uma instância de entidade.|
|nome|String|O nome de exibição de uma instância de entidade.|

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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


