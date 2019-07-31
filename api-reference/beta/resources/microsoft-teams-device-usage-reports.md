---
title: Relatórios de uso de dispositivos do Microsoft Teams
description: 'Use os relatórios de uso de dispositivos do Microsoft Teams para obter informações sobre o uso de dispositivos do Microsoft Teams em sua organização. '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0beada44b46afad1b8a51358f18259374a654f14
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966710"
---
# <a name="microsoft-teams-device-usage-reports"></a>Relatórios de uso de dispositivos do Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os relatórios de uso de dispositivos do Microsoft Teams para obter informações sobre o uso de dispositivos do Microsoft Teams em sua organização. 

## <a name="methods"></a>Métodos

| Método                                   | Tipo de retorno                              | Descrição                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário. |
| [Obter contagens de usuários](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | Obtém o número de usuários exclusivos diários por tipo de dispositivo. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | Obtém o número de usuários exclusivos por tipo de dispositivo no período de tempo selecionado. |
