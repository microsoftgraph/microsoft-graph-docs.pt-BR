---
title: Tipo de recurso userTrainingStatusInfo
description: Representa o treinamento atribuído e seu status para um usuário em simulação de ataque e treinamento.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: d9e2900bb2c72ba8100d5fe49130b7229db988ee
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757840"
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
|trainingStatus|trainingStatus|Status do treinamento atribuído ao usuário. Os possíveis valores são: `unknown`, `assigned`, `inProgress`, `completed`, `overdue`, `unknownFutureValue`.|

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

