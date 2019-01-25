---
title: Relatórios de uso de dispositivos do Microsoft Teams
description: 'Use os relatórios de uso do dispositivo Teams da Microsoft para obter ideias sobre o uso de dispositivo Teams da Microsoft em sua organização. '
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f9240f6cb310ada94f1a6694efb0da6cd691dc13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519903"
---
# <a name="microsoft-teams-device-usage-reports"></a>Relatórios de uso de dispositivos do Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os relatórios de uso do dispositivo Teams da Microsoft para obter ideias sobre o uso de dispositivo Teams da Microsoft em sua organização. 

## <a name="methods"></a>Métodos

| Método                                   | Tipo de retorno                              | Descrição                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário. |
| [Obter contagens de usuários](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | Obtém o número de usuários exclusivos diários por tipo de dispositivo. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | Obtém o número de usuários exclusivos por tipo de dispositivo no período de tempo selecionado. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
