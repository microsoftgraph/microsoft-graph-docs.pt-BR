---
title: Relatórios de atividades de usuários do Microsoft Teams
description: Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: c3dd136807e0b0aef299274fc596a2e7465ba711
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021347"
---
# <a name="microsoft-teams-user-activity-reports"></a>Relatórios de atividades de usuários do Microsoft Teams

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.

## <a name="methods"></a>Métodos

| Método                                   | Tipo de retorno                              | Descrição                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário. |
| [Obter contagens de atividades](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |
| [Obter contagens de usuários](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | Obtém o número de usuários por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |


