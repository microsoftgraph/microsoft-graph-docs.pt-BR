---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f36ed78805bc664adfbbd4ced9bc86b1444ab262
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007001"
---
# <a name="yammer-device-usage-reports"></a>Relatórios de uso de dispositivos do Yammer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os relatórios de uso do dispositivo para o Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para se envolver no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e exibir detalhes por usuário.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getyammerdeviceusageuserdetail.md) | Fluxo          | [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) | Obtenha dados sobre o uso do dispositivo Yammer por usuário. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Fluxo          | [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) | Obtenha o número de usuários por tipo de dispositivo.  |
| [Obter contagens de usuários](../api/reportroot-getyammerdeviceusageusercounts.md) | Fluxo          | [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) | Obtenha o número de usuários diários por tipo de dispositivo. |
