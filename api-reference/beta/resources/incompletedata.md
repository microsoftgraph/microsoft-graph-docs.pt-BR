---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
ms.openlocfilehash: 4319ab0f36e12ddd28ca9bb6c7bfd48043228504
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034182"
---
# <a name="incompletedata-resource-type"></a>tipo de recurso de incompleteData

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.
As propriedades dentro podem fornecer informações sobre por que não há dados incompletos.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo           | Descrição
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | O serviço não tem dados de origem antes da hora especificada.
| wasThrottled              | Booliano        | Alguns dados não foi gravados devido à atividade excessiva.

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
