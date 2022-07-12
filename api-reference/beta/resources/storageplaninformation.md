---
author: psampath
description: O recurso storagePlanInformation fornece informações sobre os planos de cota de armazenamento da unidade.
ms.date: 06/20/2018
title: StoragePlanInformation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 036da4561666bacf12f3cd7a448c9b9ba18808aa
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735940"
---
# <a name="storageplaninformation-resource-type"></a>Tipo de recurso storagePlanInformation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso storagePlanInformation** fornece informações sobre os planos de cota de armazenamento da unidade.

### <a name="json-representation"></a>Representação JSON

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

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo    | Descrição                                                             |
| :--------------- | :------ | :---------------------------------------------------------------------- |
| upgradeAvailable | Boolean | Indica se há planos de cota de armazenamento mais altos disponíveis. Somente leitura. |

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
