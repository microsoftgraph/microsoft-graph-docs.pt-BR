---
author: psampath
description: O recurso Adicionadostorageplaninformation fornece informações sobre os planos de cota de armazenamento da unidade.
ms.date: 06/20/2018
title: Adicionadostorageplaninformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d8ddb39f9f7c6443f0e669052084af27b8fd5cec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008079"
---
# <a name="storageplaninformation-resource-type"></a>tipo de recurso Adicionadostorageplaninformation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **adicionadostorageplaninformation** fornece informações sobre os planos de cota de armazenamento da unidade.

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

| Nome da propriedade     | Tipo      | Descrição                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| upgradeAvailable  | Booliano   | Indica se há planos de cota de armazenamento mais altos disponíveis. Somente leitura. |


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

