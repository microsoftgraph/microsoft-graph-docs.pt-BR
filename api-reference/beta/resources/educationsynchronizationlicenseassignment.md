---
title: tipo de recurso educationSynchronizationLicenseAssignment
description: Representa as informações de licença a serem atribuídas às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5c806b451cc7f757da09927a5732426b0971f2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500188"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>tipo de recurso educationSynchronizationLicenseAssignment

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de licença a serem atribuídas às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **appliesTo** | string | O tipo de função de usuário a ser atribuído à licença. Os valores possíveis são: `student`, `teacher`, `faculty`.         |
| **skuIds** | coleção de cadeias de caracteres |  Representa os identificadores de SKU das licenças a serem atribuídas.        |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
