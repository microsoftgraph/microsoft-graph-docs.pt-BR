---
author: psampath
description: O recurso Adicionadostorageplaninformation fornece informações sobre os planos de cota de armazenamento da unidade.
ms.date: 06/20/2018
title: Adicionadostorageplaninformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 79254efa033528bd8fd4cf66a07959a71e3fef1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520433"
---
# <a name="storageplaninformation-resource-type"></a>tipo de recurso Adicionadostorageplaninformation

Namespace: Microsoft. Graph

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

