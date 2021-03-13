---
title: Tipo complexo requestorManager
description: Identifica uma relação com outro usuário no locatário que será permitido como aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4bfd42854a55ec2daa9e380c539a25479b0e933
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761076"
---
# <a name="requestormanager-complex-type"></a>Tipo complexo requestorManager

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de aprovação de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) É um subtipo de [userSet](userset.md), no qual o valor indica que o gerente de um usuário solicitante `@odata.type` deve ser o `#microsoft.graph.requestorManager` aprovador.  Ao criar um estágio de aprovação da política de atribuição de pacote de acesso com requestorManager, inclua também outro aprovador, como um único usuário ou membro do grupo, caso o usuário solicitante não tenha um gerente.


## <a name="properties"></a>Propriedades


| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | Boolean | Para um gerente em um estágio de aprovação, indica se o gerente é um aprovador de fallback de backup. |
|managerLevel | Int32 | O nível hierárquico do gerente em relação ao solicitante. Por exemplo, o gerente direto de um solicitante teria um managerLevel de 1, enquanto o gerente do gerente do solicitante teria um managerLevel de 2. O valor padrão para managerLevel é 1. Os valores possíveis para essa propriedade variam de 1 a 2. |


## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "managerLevel": 1
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorManager complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


