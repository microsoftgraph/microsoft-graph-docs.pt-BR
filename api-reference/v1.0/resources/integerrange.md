---
title: Tipo de recurso integerRange
description: Representa um intervalo inclusivo de inteiros descrito por dois limites int64.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: aee4ebfab164e6abbbecde083ba028c4c5a98723
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516843"
---
# <a name="integerrange-resource-type"></a>Tipo de recurso integerRange

Namespace: microsoft.graph

Representa um intervalo inclusivo de inteiros descrito por dois limites int64.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|iniciar|Int64|O limite inferior inclusivo do intervalo inteiro.|
|end|Int64|O limite superior inclusivo do intervalo inteiro.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.integerRange"
}
-->
```json
{
    "start": 12345,
    "end": 12345
}
```