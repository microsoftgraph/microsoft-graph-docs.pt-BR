---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso de dispositivos do Yammer dão informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo durante um período de tempo selecionado e exibir detalhes por usuário.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 47dcdabb2230645ce2575fc573a99c37868c1919
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982429"
---
# <a name="yammer-device-usage-reports"></a>Relatórios de uso de dispositivos do Yammer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os relatórios de uso de dispositivos do Yammer dão informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo durante um período de tempo selecionado e exibir detalhes por usuário.

> **Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira [relatórios do Microsoft 365 - uso de dispositivos do Yammer.](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getyammerdeviceusageuserdetail.md) | Fluxo          | [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) | Obtenha dados sobre o uso do dispositivo Yammer por usuário. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Fluxo          | [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) | Obtenha o número de usuários por tipo de dispositivo.  |
| [Obter contagens de usuários](../api/reportroot-getyammerdeviceusageusercounts.md) | Fluxo          | [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) | Obtenha o número de usuários diários por tipo de dispositivo. |


