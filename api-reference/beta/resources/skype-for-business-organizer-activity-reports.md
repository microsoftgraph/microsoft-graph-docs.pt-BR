---
title: Relatórios de atividades do organizador do Skype for Business
description: Você pode obter detalhes sobre a atividade de conferências organizadas em toda a sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: f12d8060b895a6e16c2c48ed3b902d0322357c1e
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390157"
---
# <a name="skype-for-business-organizer-activity-reports"></a>Relatórios de atividades do organizador do Skype for Business

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter detalhes sobre a atividade de conferências organizadas em toda a sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, consulte Microsoft 365 relatórios - Skype for Business atividade do organizador [da conferência.](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter contagens de atividade](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | Fluxo          | Fluxo           | Obtenha tendências de uso do número e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | Fluxo          | Fluxo           | Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft. |
| [Obter contagens de minutos](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | Fluxo          | Fluxo           | Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft. |


