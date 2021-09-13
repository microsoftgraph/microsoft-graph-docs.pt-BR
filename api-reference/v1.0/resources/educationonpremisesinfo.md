---
title: Tipo de recurso educationOnPremisesInfo
description: Informações adicionais usadas para associar uma conta de usuário local do Active Directory ao objeto de usuário do Azure AD.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ace4f32edf7a708debea828bfc510aec630a7100
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078886"
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
