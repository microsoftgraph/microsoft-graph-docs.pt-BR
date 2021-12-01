---
title: Tipo complexo requestorManager
description: Identifica uma relação com outro usuário no locatário que será permitido como aprovador.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a4f82b55438fe2e077cca299d55aa6af2c0fecb
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242270"
---
# <a name="requestormanager-complex-type"></a>Tipo complexo requestorManager

Namespace: microsoft.graph

Usado nas configurações de aprovação de uma política de atribuição de pacote de acesso.
É um subtipo de [subjectSet](subjectset.md), no qual o valor indica que o gerente de um usuário solicitante `@odata.type` deve ser o `#microsoft.graph.requestorManager` aprovador.  Ao criar um estágio de aprovação da política de atribuição de pacote de acesso com requestorManager, inclua também outro aprovador, como um único usuário ou membro do grupo, caso o usuário solicitante não tenha um gerente.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|managerLevel|Int32|O nível hierárquico do gerente em relação ao solicitante. Por exemplo, o gerente direto de um solicitante teria um managerLevel de 1, enquanto o gerente do gerente do solicitante teria um managerLevel de 2. O valor padrão para managerLevel é 1. Os valores possíveis para essa propriedade variam de 1 a 2. |

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requestorManager",
  "managerLevel": "Integer"
}
```


