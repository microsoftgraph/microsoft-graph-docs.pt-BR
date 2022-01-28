---
title: tipo de recurso teamworkAccountConfiguration
description: Representa os detalhes sobre a configuração da conta para um Salas do Microsoft Teams dispositivo.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5b3fc0edb85380f8a858bf6b9910a819443bfb8b
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262275"
---
# <a name="teamworkaccountconfiguration-resource-type"></a>tipo de recurso teamworkAccountConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre a configuração da conta de um Salas do Microsoft Teams [dispositivo](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|onPremisesCalendarSyncConfiguration|[teamworkOnPremisesCalendarSyncConfiguration](../resources/teamworkonpremisescalendarsyncconfiguration.md)|A conta usada para sincronizar o calendário.|
|supportedClient|teamworkSupportedClient|O cliente com suporte para Salas do Teams dispositivos. Os valores possíveis são: `unknown`, `skypeDefaultAndTeams`, `teamsDefaultAndSkype`, `skypeOnly`, `teamsOnly`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkAccountConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkAccountConfiguration",
  "onPremisesCalendarSyncConfiguration": {
    "@odata.type": "microsoft.graph.teamworkOnPremisesCalendarSyncConfiguration"
  },
  "supportedClient": "String"
}
```

