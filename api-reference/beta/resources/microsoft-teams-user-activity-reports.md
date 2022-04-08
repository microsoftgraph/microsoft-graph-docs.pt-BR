---
title: Relatórios de atividades de usuários do Microsoft Teams
description: Use os Microsoft Teams de atividades do usuário para obter insights sobre a Microsoft Teams do usuário em sua organização.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: d49f7c0ebccbc70f10460673d73aab3794283195
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704230"
---
# <a name="microsoft-teams-user-activity-reports"></a>Relatórios de atividades de usuários do Microsoft Teams

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use os Microsoft Teams de atividades do usuário para obter insights sobre a Microsoft Teams do usuário em sua organização.

## <a name="methods"></a>Métodos

| Método                                                       | Tipo de retorno | Descrição                                                  |
| :----------------------------------------------------------- | :---------- | :----------------------------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getteamsuseractivityuserdetail.md) | Fluxo      | Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.     |
| [Obter contagens de atividades](../api/reportroot-getteamsuseractivitycounts.md) | Fluxo      | Obtém o número de atividades do Microsoft Teams por tipo de atividade. As atividades são executadas por Microsoft Teams licenciados. |
| [Obter contagens totais de atividades](../api/reportroot-getteamsuseractivitytotalcounts.md) | Fluxo      | Obtém o número de atividades do Microsoft Teams por tipo de atividade. As atividades são executadas Microsoft Teams usuários licenciados ou não licenciados. |
| [Obter contagens de usuários](../api/reportroot-getteamsuseractivityusercounts.md) | Fluxo      | Obter o número de usuários Microsoft Teams licenciados por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |
| [Obter contagens totais de usuários](../api/reportroot-getteamsuseractivitytotalusercounts.md) | Stream      | Obtenha o número de Microsoft Teams usuários licenciados ou não licenciados por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões. |
| [Obter contagens de usuários de distribuição](../api/reportroot-getteamsuseractivitydistributionusercounts.md) | Fluxo      | Obtenha o número de usuários Microsoft Teams licenciados por tipo de atividade durante o período selecionado. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões. |
| [Obter contagens de usuários totais de distribuição](../api/reportroot-getteamsuseractivitydistributiontotalusercounts.md) | Stream      | Obtenha o número de Microsoft Teams usuários licenciados ou não licenciados por tipo de atividade durante o período selecionado. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas e reuniões. |
| [Obter contagens totais de atividades de distribuição](../api/reportroot-getteamsuseractivitytotaldistributioncounts.md) | Stream      | Obtenha o número de atividades Microsoft Teams usuário durante o período selecionado. Os tipos de atividade são mensagens de chat de equipe, mensagens de chat privadas, chamadas, reuniões, reuniões organizadas, reuniões atendidas, duração do áudio, duração do vídeo, duração do compartilhamento de tela, mensagens de postagem e mensagens de resposta. |

