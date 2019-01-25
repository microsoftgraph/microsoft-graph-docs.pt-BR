---
title: Relatórios de uso de dispositivos do Yammer
description: Os relatórios de uso de dispositivos paro Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para conectar no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e visualizar dados por usuário.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f5b24d6d235a8719f5f4b7df0389b5e5971dd8cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521863"
---
# <a name="yammer-device-usage-reports"></a>Relatórios de uso de dispositivos do Yammer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os relatórios de uso de dispositivos paro Yammer fornecem informações sobre quais dispositivos seus usuários utilizam para conectar no Yammer. Você pode exibir o número de usuários por tipo de dispositivo em um período de tempo selecionado e visualizar dados por usuário.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream          | [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) | Obtenha dados sobre o uso do dispositivo Yammer por usuário. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Fluxo          | [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) | Obtenha o número de usuários por tipo de dispositivo.  |
| [Obter contagens de usuários](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream          | [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) | Obtenha o número de usuários diários por tipo de dispositivo. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
