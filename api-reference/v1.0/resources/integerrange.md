---
title: Tipo de recurso integerRange
description: Representa um intervalo inclusivo de inteiros descrito por dois limites int64.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 6af69a7184a88d8540b45b35a58875b5d2934712fa0915bb0d1e59df2623697d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146857"
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