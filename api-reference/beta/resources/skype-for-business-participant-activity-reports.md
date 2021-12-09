---
title: Relatórios de atividades do participante do Skype for Business
description: Você pode obter detalhes sobre a atividade de conferência em toda a sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: fd36531048d70e33ac2ac2d805ccff8068dd0d40
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390183"
---
# <a name="skype-for-business-participant-activity-reports"></a>Relatórios de atividades do participante do Skype for Business

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter detalhes sobre a atividade de conferência em toda a sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Skype for Business atividade](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)do participante da conferência .

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter contagens de atividade](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | Fluxo          | Fluxo           | Obtenha tendências de uso do número e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | Fluxo          | Fluxo           | Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros. |
| [Obter contagens de minutos](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | Fluxo          | Fluxo           | Obtenha as tendências de uso da duração em minutos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem áudio/vídeo. |


