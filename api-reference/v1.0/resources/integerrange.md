---
title: Tipo de recurso integerRange
description: Representa um intervalo inclusivo de inteiros descritos por dois limites Int64.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: b869d99fc4fef8b6804a3559ddd21e7d661ea32b
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899432"
---
# <a name="integerrange-resource-type"></a>Tipo de recurso integerRange

Namespace: microsoft.graph

Representa um intervalo inclusivo de inteiros descritos por dois limites Int64.

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
