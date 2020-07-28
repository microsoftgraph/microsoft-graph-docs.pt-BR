---
title: tipo de recurso educationSynchronizationLicenseAssignment
description: Representa as informações de licença a serem atribuídas às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9d46e19c1869f7dff96a563dd54b1b9f303ce85a
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434960"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>tipo de recurso educationSynchronizationLicenseAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de licença a serem atribuídas às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo              | Descrição                                                                                    |
| :-------- | :---------------- | :--------------------------------------------------------------------------------------------- |
| appliesTo | Cadeia de caracteres            | O tipo de função de usuário a ser atribuído à licença. Os valores possíveis são: `student`, `teacher`, `faculty`. |
| skuIds    | Conjunto de cadeias de caracteres | Representa os identificadores de SKU das licenças a serem atribuídas.                                      |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "skuIds": ["String"]
}
```
