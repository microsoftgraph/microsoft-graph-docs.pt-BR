---
title: Tipo de recurso userTrainingStatusInfo
description: Representa o treinamento atribuído e seu status para um usuário em simulação de ataque e treinamento.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 82b0c6b1de49c9b8eb0572dab33fca8c90e2b6fe
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979476"
---
# <a name="usertrainingstatusinfo-resource-type"></a>Tipo de recurso userTrainingStatusInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um treinamento atribuído e seu status para um usuário em simulação de ataque e treinamento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedDateTime|DateTimeOffset|Data e hora de atribuição do treinamento para o usuário.|
|completionDateTime|DateTimeOffset|Data e hora de conclusão do treinamento pelo usuário.|
|displayName|Cadeia de caracteres|Nome de exibição do treinamento atribuído.|
|trainingStatus|trainingStatus|Status do treinamento atribuído ao usuário. Os valores possíveis são: `unknown`, `assigned`, `inProgress`, `completed`, `overdue`, `notCompleted`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTrainingStatusInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTrainingStatusInfo",
  "assignedDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "trainingStatus": "String",
  "displayName": "String"
}
```

