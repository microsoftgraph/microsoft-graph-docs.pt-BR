---
title: tipo de recurso de audioDuckingConfiguration
description: Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 713e7012381bf6b727321494f81e75c88c66ebe6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891557"
---
# <a name="audioduckingconfiguration-resource-type"></a>tipo de recurso de audioDuckingConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo     | Descrição                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| lowerLevel    | Int64    | O volume das fontes em % quando as fontes estão sendo ducked.             |
| rampActive    | Int64    | A quantidade de tempo (em milissegundos) que leva para fontes ducked "desaparecer". |
| rampInactive  | Int64    | A quantidade de tempo (em milissegundos) que leva para ducked fontes para "desaparecer".  |
| upperLevel    | Int64    | O volume das fontes em % quando as fontes não estão sendo ducked.         |

> **Observação:** Duração conheça não pode ser mais de 5.000 milissegundos.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
