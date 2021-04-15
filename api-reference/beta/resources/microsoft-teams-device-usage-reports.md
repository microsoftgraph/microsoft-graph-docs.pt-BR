---
title: Relatórios de uso de dispositivos do Microsoft Teams
description: 'Use os relatórios de uso de dispositivo do Microsoft Teams para obter informações sobre o uso de dispositivos do Microsoft Teams em sua organização. '
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b9a4d2ab3034281970a3e342aa0a2d78e53678e5
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766109"
---
# <a name="microsoft-teams-device-usage-reports"></a>Relatórios de uso de dispositivos do Microsoft Teams

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os relatórios de uso de dispositivo do Microsoft Teams para obter informações sobre o uso de dispositivos do Microsoft Teams em sua organização. 

## <a name="methods"></a>Métodos

| Método                                                       | Tipo de retorno                                                  | Descrição                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.      |
| [Obter contagens de usuários](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | Obter o número de usuários licenciados diários exclusivos do Microsoft Teams por tipo de dispositivo. |
| [Obter contagens totais de usuários](../api/reportroot-getteamsdeviceusagetotalusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | Obter o número de usuários exclusivos exclusivos do Microsoft Teams licenciados ou não licenciados por tipo de dispositivo. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | Obter o número de usuários licenciados exclusivos do Microsoft Teams por tipo de dispositivo durante o período de tempo selecionado. |
| [Obter contagens totais de usuários de distribuição](../api/reportroot-getteamsdeviceusagedistributiontotalusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | Obter o número de usuários exclusivos licenciados ou não licenciados do Microsoft Teams por tipo de dispositivo durante o período de tempo selecionado. |


