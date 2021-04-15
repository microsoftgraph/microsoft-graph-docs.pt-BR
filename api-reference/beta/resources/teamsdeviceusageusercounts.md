---
title: Tipo de recurso teamsDeviceUsageUserCounts
description: Representa o número de usuários diários por tipo de dispositivo.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d7b813727a5ac9b2f7547e108bad8ee455d206b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766571"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a>Tipo de recurso teamsDeviceUsageUserCounts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o número de usuários diários por tipo de dispositivo.

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                                                  |
| :---------------- | :----- | ------------------------------------------------------------ |
| reportRefreshDate | Data   | A data mais recente do conteúdo.                              |
| web               | Int64  | O número de usuários que estavam ativos no cliente Web do Teams em dispositivos. |
| windowsPhone      | Int64  | O número de usuários que estavam ativos no cliente móvel do Teams para windows phone. |
| androidPhone      | Int64  | O número de usuários que estavam ativos no cliente móvel do Teams para Android. |
| ios               | Int64  | O número de usuários que estavam ativos no cliente móvel do Teams para iOS. |
| mac               | Int64  | O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador macOS. |
| windows           | Int64  | O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador baseado no Windows. |
| chromeOS          | Int64  | O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador ChromeOS. |
| linux             | Int64  | O número de usuários que estavam ativos no cliente de área de trabalho do Teams em um computador Linux. |
| reportDate        | Data   | A data em que os usuários realizaram as atividades.        |
| reportPeriod      | String | O número de dias que o relatório aborda.                        |

## <a name="representation"></a>representation

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "chromeOS": 1024, 
  "linux": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


