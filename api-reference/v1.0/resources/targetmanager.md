---
title: Tipo de recurso targetManager
description: Tipo complexo de gerenciamento de direitos para indicar o gerente, incluindo gerentes indiretos de um usuário podem solicitar em nome desse usuário.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 06859aea4cc966ca25ded6dc8e972adf6ca2a600
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608259"
---
# <a name="targetmanager-complex-type"></a>tipo complexo targetManager

Namespace: microsoft.graph

Usado em uma política de atribuição de pacote de acesso, esse tipo herda de [subjectSet](../resources/subjectset.md) e indica o gerente, incluindo gerentes indiretos de um usuário podem solicitar em nome desse usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|managerLevel|Int32|Nível do gerente, entre 1 e 4. O gerente direto é 1.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.targetManager"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetManager",
  "managerLevel": "Integer"
}
```


