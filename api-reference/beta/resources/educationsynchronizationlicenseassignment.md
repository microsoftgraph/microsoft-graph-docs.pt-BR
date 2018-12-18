---
title: tipo de recurso de educationSynchronizationLicenseAssignment
description: Representa as informações de licença para atribuir às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.
author: mmast-msft
ms.openlocfilehash: 478d939c8f4c6a0bc1971d66afc4ecc7ae640e39
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344391"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>tipo de recurso de educationSynchronizationLicenseAssignment

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa as informações de licença para atribuir às contas de usuário. O recurso será usado para configurar atribuições de licença ao criar novas contas de usuário.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **appliesTo** | string | O tipo de função de usuário para atribuir a licença. Os valores possíveis são: `student` e `teacher`.         |
| **skuIds** | coleção de sequências de caracteres |  Representa os identificadores SKU das licenças para atribuir.        |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
