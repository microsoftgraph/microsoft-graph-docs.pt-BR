---
author: learafa
description: O recurso Adicionadostorageplaninformation fornece informações sobre os planos de cota de armazenamento da unidade.
title: Adicionadostorageplaninformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: b8b4778a4726c227bfe79ad13ecb14507b13a889
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036951"
---
# <a name="storageplaninformation-resource-type"></a>tipo de recurso Adicionadostorageplaninformation

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


