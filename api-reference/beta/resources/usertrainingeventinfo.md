---
title: Tipo de recurso userTrainingEventInfo
description: Representa eventos de um treinamento atribuído a um usuário em uma campanha de simulação e treinamento de ataque.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1a33cba93e61752d33b9829871b3280955895360
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758232"
---
# <a name="usertrainingeventinfo-resource-type"></a>Tipo de recurso userTrainingEventInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa eventos de um treinamento atribuído a um usuário em uma campanha de simulação e treinamento de ataque. Os eventos de treinamento incluem atribuir o treinamento, atualizar o treinamento em andamento e concluir o treinamento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição do treinamento.|
|latestTrainingStatus|trainingStatus|Status mais recente do treinamento atribuído ao usuário. Os possíveis valores são: `unknown`, `assigned`, `inProgress`, `completed`, `overdue`, `unknownFutureValue`.|
|trainingAssignedProperties|[userTrainingContentEventInfo](../resources/usertrainingcontenteventinfo.md)|Detalhes do evento do treinamento quando ele foi atribuído ao usuário.|
|trainingCompletedProperties|[userTrainingContentEventInfo](../resources/usertrainingcontenteventinfo.md)|Detalhes do evento do treinamento quando ele foi concluído pelo usuário.|
|trainingUpdatedProperties|[userTrainingContentEventInfo](../resources/usertrainingcontenteventinfo.md)|Detalhes do evento do treinamento quando ele foi atualizado/em andamento pelo usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTrainingEventInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTrainingEventInfo",
  "displayName": "String",
  "latestTrainingStatus": "String",
  "trainingAssignedProperties": {
    "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
  },
  "trainingUpdatedProperties": {
    "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
  },
  "trainingCompletedProperties": {
    "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
  }
}
```

