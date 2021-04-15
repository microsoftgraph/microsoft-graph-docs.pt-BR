---
title: Tipo de recurso teamsDeviceUsageDistributionUserCounts
description: Representa o número de usuários por tipo de dispositivo durante o período de tempo selecionado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d1c716a4be9ab6ffac7b37484d7cb8bc8f01ee9
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766564"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a>Tipo de recurso teamsDeviceUsageDistributionUserCounts

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o número de usuários por tipo de dispositivo durante o período de tempo selecionado.

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
| reportPeriod      | String | O número de dias que o relatório aborda.                        |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```


