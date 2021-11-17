---
title: Relatórios de atividades de usuários do Microsoft Teams
description: Use os Microsoft Teams de atividades do usuário para obter informações sobre a Microsoft Teams do usuário em sua organização.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 46ab4747f5ce4e38ab57a56e54528f4c3dfb9360
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044677"
---
# <a name="microsoft-teams-user-activity-reports"></a>Relatórios de atividades de usuários do Microsoft Teams

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os Microsoft Teams de atividades do usuário para obter informações sobre a Microsoft Teams do usuário em sua organização.

## <a name="methods"></a>Métodos

| Método                                                       | Tipo de retorno | Descrição                                                  |
| :----------------------------------------------------------- | :---------- | :----------------------------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getteamsuseractivityuserdetail.md) | Fluxo      | Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.     |
| [Obter contagens de atividades](../api/reportroot-getteamsuseractivitycounts.md) | Fluxo      | Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. As atividades são executadas por Microsoft Teams usuários licenciados. |
| [Obter contagens totais de atividade](../api/reportroot-getteamsuseractivitytotalcounts.md) | Fluxo      | Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. As atividades são executadas por Microsoft Teams usuários licenciados ou não licenciados. |
| [Obter contagens de usuários](../api/reportroot-getteamsuseractivityusercounts.md) | Fluxo      | Obter o número de usuários Microsoft Teams licenciados por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |
| [Obter contagens totais de usuários](../api/reportroot-getteamsuseractivitytotalusercounts.md) | Stream      | Obter o número de usuários Microsoft Teams licenciados ou não licenciados por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getteamsuseractivitydistributionusercounts.md) | Fluxo      | Obter o número de usuários Microsoft Teams licenciados por tipo de atividade durante o período selecionado. Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões. |
| [Obter contagens totais de usuários de distribuição](../api/reportroot-getteamsuseractivitydistributiontotalusercounts.md) | Stream      | Obter o número de usuários Microsoft Teams licenciados ou não licenciados por tipo de atividade durante o período selecionado. Os tipos de atividade são o número de mensagens de chat das equipes, mensagens de chat privadas, chamadas e reuniões. |


