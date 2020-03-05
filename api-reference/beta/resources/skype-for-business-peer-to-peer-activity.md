---
title: Relatórios de atividades ponto a ponto Skype for Business
description: Você pode obter detalhes sobre as atividades ponto a ponto em toda a organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 855f34d7ccdc9969bdca57e60ef5b59efb37eeac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520461"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a>Relatórios de atividades ponto a ponto Skype for Business

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter detalhes sobre as atividades ponto a ponto em toda a organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade ponto a ponto do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter contagens de atividade](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | Stream          | [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) | Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | Fluxo          | [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto. |
| [Obter contagens de minutos](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | Fluxo          | [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização. Tipos de sessões incluem áudio e vídeo. |
