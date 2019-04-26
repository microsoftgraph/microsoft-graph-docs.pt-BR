---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: Adicionadostorageplaninformation
localization_priority: Normal
ms.openlocfilehash: 3911d3af5f2149d1043ed246e7c11d287c840842
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342916"
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
| upgradeAvailable  | Boolean   | Indica se há planos de cota de armazenamento mais altos disponíveis. Somente leitura. |


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

