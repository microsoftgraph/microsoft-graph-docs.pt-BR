---
title: Relatórios de atividades de usuários do Microsoft Teams
description: Use os relatórios de atividade do usuário do Microsoft Teams para obter informações sobre a atividade do usuário do Microsoft Teams em sua organização.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 97a32ce99eab154a99a97d9c9dab7fc49d4a7a1d
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766116"
---
# <a name="microsoft-teams-user-activity-reports"></a>Relatórios de atividades de usuários do Microsoft Teams

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os relatórios de atividade do usuário do Microsoft Teams para obter informações sobre a atividade do usuário do Microsoft Teams em sua organização.

## <a name="methods"></a>Métodos

| Método                                                       | Tipo de retorno                                                  | Descrição                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.     |
| [Obter contagens de atividades](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. As atividades são executadas por usuários licenciados do Microsoft Teams. |
| [Obter contagens totais de atividade](../api/reportroot-getteamsuseractivitytotalcounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. As atividades são executadas por usuários licenciados ou não licenciados do Microsoft Teams. |
| [Obter contagens de usuários](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | Obter o número de usuários licenciados do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |
| [Obter contagens totais de usuários](../api/reportroot-getteamsuseractivitytotalusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | Obter o número de usuários licenciados ou não licenciados do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getteamsuseractivitydistributionusercounts.md) | [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) | Obter o número de usuários licenciados do Microsoft Teams por tipo de atividade durante o período selecionado. Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões. |
| [Obter contagens totais de usuários de distribuição](../api/reportroot-getteamsuseractivitydistributiontotalusercounts.md) | [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) | Obter o número de usuários licenciados ou não licenciados do Microsoft Teams por tipo de atividade durante o período selecionado. Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões. |


