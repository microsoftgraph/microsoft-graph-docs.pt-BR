---
author: daspek
title: Tipo de recurso incompleteData
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f4d8c852a08780ecc0f48ac8a1dcef11b246673c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128309"
---
# <a name="incompletedata-resource-type"></a>Tipo de recurso incompleteData

Namespace: microsoft.graph

A **faceta incompleteData** indica que um recurso foi gerado com dados incompletos.
As propriedades dentro podem fornecer informações sobre por que os dados estão incompletos.

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo           | Descrição
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | O serviço não tem dados de origem antes do horário especificado.
| wasThrottled              | Boolean        | Alguns dados não foram registrados devido a atividades excessivas.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->

