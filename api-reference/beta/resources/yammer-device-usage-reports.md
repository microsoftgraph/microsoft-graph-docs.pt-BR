---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso de dispositivos paro Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para conectar no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e visualizar dados por usuário.
ms.openlocfilehash: da94fb91d3feb17052cf02b09e27cdc70b7f734b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039134"
---
# <a name="yammer-device-usage-reports"></a>Relatórios de uso de dispositivos do Yammer

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção. Essas APIs não são suportadas na China Microsoft Graph operado pela 21Vianet.

Os relatórios de uso de dispositivos paro Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para conectar no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e visualizar dados por usuário.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getyammerdeviceusageuserdetail.md) | Fluxo          | [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) | Obtenha dados sobre o uso do dispositivo Yammer por usuário. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Fluxo          | [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) | Obtenha o número de usuários por tipo de dispositivo.  |
| [Obter contagens de usuários](../api/reportroot-getyammerdeviceusageusercounts.md) | Fluxo          | [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) | Obtenha o número de usuários diários por tipo de dispositivo. |
