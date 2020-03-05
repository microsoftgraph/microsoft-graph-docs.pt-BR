---
title: tipo de recurso de email
description: tipo de recurso de email
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a18d72fb44f373b6cee1047cc2eed5f0c18a1d0e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523076"
---
# <a name="itememail-resource-type"></a>tipo de recurso de email

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre endereços de email associados ao usuário.

## <a name="methods"></a>Métodos

| Método                                   | Tipo de retorno               | Descrição                                            |
|:-----------------------------------------|:--------------------------|:-------------------------------------------------------|
| [Get](../api/itememail-get.md) | [Email](itememail.md) | Ler propriedades e relações de um objeto item de **email** . |
| [Update](../api/itememail-update.md)     | [Email](itememail.md) | Atualize um objeto de **email** .                               |
| [Delete](../api/itememail-delete.md)     | None                      | Excluir um objeto de **email** .                               |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|address       |Cadeia de caracteres       | O próprio endereço de email.                                                 |
|displayName   |Cadeia de caracteres       | O nome ou rótulo que um usuário associou a um endereço de email específico.  |
|type          |cadeia de caracteres       | Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.      |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": ""
}-->

```json
{
  "address": "String",
  "displayName": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemEmail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
