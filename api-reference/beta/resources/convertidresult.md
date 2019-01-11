---
title: tipo de recurso de convertIdResult
description: O resultado de uma conversão de formato de ID realizada pela função translateExchangeIds.
localization_priority: Normal
ms.openlocfilehash: 7e1878de3d3b7ddee36d799c928d6a130b578200
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821452"
---
# <a name="convertidresult-resource-type"></a>tipo de recurso de convertIdResult

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O resultado de uma conversão de formato de ID realizada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| sourceId | Cadeia de caracteres | O identificador que foi convertido. Esse valor é o identificador original, não convertido. |
| Alvo | Cadeia de caracteres | O identificador convertido. Este valor não estiver presente, se a conversão falhou. |
| errorDetails | [Erro genérico](genericerror.md) | Um objeto de erro que indica o motivo da falha de conversão. Este valor não estiver presente, se a conversão foi bem-sucedida. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
