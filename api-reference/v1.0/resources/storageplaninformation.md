---
author: learafa
description: O recurso storagePlanInformation fornece informações sobre os planos de cota de armazenamento da unidade.
title: StoragePlanInformation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: a26704495253d9dd33f4bcb37395b927ca8a4342
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136324"
---
# <a name="storageplaninformation-resource-type"></a>Tipo de recurso storagePlanInformation

Namespace: microsoft.graph

Fornece informações sobre os planos de cota de armazenamento da unidade.

## <a name="properties"></a>Propriedades

| Nome da propriedade     | Tipo      | Descrição                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| **upgradeAvailable**  | Boolean   | Indica se há planos de cota de armazenamento mais altos disponíveis. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```

<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": []
}
-->


