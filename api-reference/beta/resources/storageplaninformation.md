---
author: psampath
description: O recurso storagePlanInformation fornece informações sobre os planos de cota de armazenamento da unidade.
ms.date: 06/20/2018
title: StoragePlanInformation
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: db5707686f6104d8d9004696094c0bcc22066f5a
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723267"
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
| upgradeAvailable | Booliano | Indica se há planos de cota de armazenamento mais altos disponíveis. Somente leitura. |

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
