---
title: Tipo de recurso integerRange
description: Representa um intervalo inclusivo de inteiros descrito por dois limites int64.
author: nilakhan
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 31661802fa198790e4d30f2da58ac11c86f19b6e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036477"
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
