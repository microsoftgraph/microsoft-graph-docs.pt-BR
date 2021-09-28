---
title: tipo de recurso assignedTrainingInfo
description: Representa as informações do treinamento atribuído em uma campanha de simulação e treinamento de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 15caed31f7db60980e453e942653820dc8b348bc
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979500"
---
# <a name="assignedtraininginfo-resource-type"></a>tipo de recurso assignedTrainingInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações de atribuição de um treinamento em uma campanha de simulação e treinamento de ataque.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedUserCount|Int32|Número de usuários que foram atribuídos ao treinamento em uma campanha de simulação e treinamento de ataque.|
|completedUserCount|Int32|Número de usuários que concluíram o treinamento em uma campanha de simulação e treinamento de ataque.|
|displayName|Cadeia de caracteres|Exibir o nome do treinamento em uma campanha de simulação e treinamento de ataque.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignedTrainingInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignedTrainingInfo",
  "assignedUserCount": "Integer",
  "completedUserCount": "Integer",
  "displayName": "String"
}
```

