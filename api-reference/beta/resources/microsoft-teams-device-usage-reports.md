---
title: Relatórios de uso de dispositivos do Microsoft Teams
description: 'Use os relatórios de uso de dispositivos do Microsoft Teams para obter informações sobre o uso de dispositivos do Microsoft Teams em sua organização. '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0f1d1776a8e4065be46e786bd84313fb04e4cb0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522635"
---
# <a name="microsoft-teams-device-usage-reports"></a>Relatórios de uso de dispositivos do Microsoft Teams

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os relatórios de uso de dispositivos do Microsoft Teams para obter informações sobre o uso de dispositivos do Microsoft Teams em sua organização. 

## <a name="methods"></a>Métodos

| Método                                   | Tipo de retorno                              | Descrição                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário. |
| [Obter contagens de usuários](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | Obtém o número de usuários exclusivos diários por tipo de dispositivo. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | Obtém o número de usuários exclusivos por tipo de dispositivo no período de tempo selecionado. |
