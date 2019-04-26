---
title: Relatórios de atividades de usuários do Microsoft Teams
description: Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: f88d1c9d568ce3fbbf9bfe19abaf637065d37b8c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342202"
---
# <a name="microsoft-teams-user-activity-reports"></a>Relatórios de atividades de usuários do Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os relatórios de atividades do usuário do Microsoft Teams para obter informações sobre a atividade de usuário do Microsoft Teams em sua organização.

## <a name="methods"></a>Métodos

| Método                                   | Tipo de retorno                              | Descrição                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário. |
| [Obter contagens de atividades](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |
| [Obter contagens de usuários](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | Obtém o número de usuários por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |
