---
author: swapnil1993
title: Tipo de recurso termColumn
description: O recurso termColumn indica que os valores da coluna contêm dados de taxonomia.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: fcdad019f3eb2496116767e560f63a4668ed7508
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720862"
---
# <a name="termcolumn-resource-type"></a>Tipo de recurso termColumn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Indica que os valores da coluna contêm dados de taxonomia.

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo                           | Descrição                                                               |
| :--------------------- | :----------------------------- | :------------------------------------------------------------------------ |
| allowMultipleValues    | Boolean                        | Especifica se a coluna permitirá mais de um valor               |
| parentTerm             | microsoft.graph.termStore.term | Especifica o guid do termo cujos filhos podem ser selecionados como o valor da coluna. |
| showFullyQualifiedName | Booliano                        | Especifica se o caminho do termo inteiro será exibido ou somente o rótulo do termo. |
| termSet                | microsoft.graph.termStore.set  | Termset cujos filhos podem ser selecionados como o valor da coluna.                 |

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um **recurso termColumn** .

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "parentTerm": { "@type": "microsoft.graph.termStore.term" },
    "showFullyQualifiedName": false,
    "termSet": { "@type": "microsoft.graph.termStore.set" }
}
```
