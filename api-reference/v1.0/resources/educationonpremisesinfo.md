---
title: Tipo de recurso educationOnPremisesInfo
description: Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4c5da3180b1c15f2363bfd651d0f4e3d68f41b60
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232128"
---
# <a name="educationonpremisesinfo-resource-type"></a>Tipo de recurso educationOnPremisesInfo

Namespace: microsoft.graph

Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                                |
| :---------- | :----- | :--------------------------------------------------------- |
| immutableId | String | Identificador exclusivo do objeto do usuário no Active Directory. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOnPremisesInfo",
  "immutableId": "String"
}
```
