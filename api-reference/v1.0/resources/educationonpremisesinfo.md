---
title: Tipo de recurso educationOnPremisesInfo
description: Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c461c63309588fc01fef94fb53a3b9c6e0f2722858f1baaa93a663804e344b7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182529"
---
# <a name="educationonpremisesinfo-resource-type"></a>Tipo de recurso educationOnPremisesInfo

Namespace: microsoft.graph

Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo   | Descrição                                                |
| :---------- | :----- | :--------------------------------------------------------- |
| immutableId | Cadeia de caracteres | Identificador exclusivo do objeto do usuário no Active Directory. |

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
