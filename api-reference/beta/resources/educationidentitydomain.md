---
title: tipo de recurso de educationIdentityDomain
description: 'Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence. O recurso de domínio é parte da configuração de criação de identidade. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 280ae1a65e0c14e7960d316cc21154e405f2ee0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982026"
---
# <a name="educationidentitydomain-resource-type"></a>tipo de recurso de educationIdentityDomain

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o mapeamento entre um tipo de usuário de educação e o domínio em que a conta do usuário pertence. O recurso de domínio é parte da [configuração de criação de identidade](educationidentitycreationconfiguration.md). 

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **appliesTo** | string |  O tipo de função de usuário para atribuir a licença. Os valores possíveis são: `student` e `teacher`.      |
| **name** | string |  Representa o domínio da conta de usuário.         |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "name": "String"
}
```
