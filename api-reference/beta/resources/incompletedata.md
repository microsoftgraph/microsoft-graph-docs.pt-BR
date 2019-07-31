---
author: daspek
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 23d78fa3605259031fc2c408e93a0461bb12cb28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006280"
---
# <a name="incompletedata-resource-type"></a>tipo de recurso incompleteData

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.
As propriedades dentro podem fornecer informações sobre o motivo pelo qual há dados incompletos.

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
| missingDataBeforeDateTime | DateTimeOffset | O serviço não tem dados de origem antes do tempo especificado.
| wasThrottled              | Booliano        | Alguns dados não foram gravados devido à atividade excessiva.

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
