---
title: tipo de recurso printerShare
description: Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a44cac259e9be653ca0e7b21c81b6c72224268b1
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895482"
---
# <a name="printershare-resource-type"></a>tipo de recurso printerShare

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar printerShares](../api/print-list-printershares.md) | coleção [printerShare](printershare.md) | Obtenha uma lista de compartilhamentos de impressora no locatário. |
| [Obter printerShare](../api/printershare-get.md) | [printerShare](printershare.md) | Ler propriedades e relações de um objeto printerShare. |
| [Update](../api/printershare-update.md) | [printerShare](printershare.md) | Atualizar um objeto printerShare. |
| [Delete](../api/printershare-delete.md) | Nenhum | Descompartilhar uma impressora. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador do printerShare. Somente leitura.|
|name|String|O nome do compartilhamento de impressora que os clientes de impressão devem exibir.|
|createdDateTime|DateTimeOffset|O DateTimeOffset quando o compartilhamento da impressora foi criado. Somente leitura.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|impressora|[impressora](printer.md)|A impressora à qual esse compartilhamento de impressora está relacionado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->