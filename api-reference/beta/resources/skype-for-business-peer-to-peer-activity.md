---
title: Relatórios de atividades ponto a ponto Skype for Business
description: Você pode obter detalhes sobre a atividade ponto a ponto em toda a sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 2d0ccd9af6989ccb1a14f07818e4647e7cb2366a
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390023"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a>Relatórios de atividades ponto a ponto Skype for Business

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter detalhes sobre a atividade ponto a ponto em toda a sua organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Skype for Business atividade ponto a ponto](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter contagens de atividade](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | Fluxo          | Fluxo           | Obtenha tendências de uso no número e tipo de sessões realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | Fluxo          | Fluxo           | Obtenha tendências de uso do número de usuários únicos e o tipo de sessões ponto a ponto realizadas em sua organização. Os tipos de sessões incluem mensagens instantâneas, áudio, vídeo, compartilhamento de aplicativos e transferência de arquivos em sessões ponto a ponto. |
| [Obter contagens de minutos](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | Fluxo          | Fluxo           | Obtenha tendências de uso da duração em minutos e tipo de sessões ponto a ponto realizadas em sua organização. Tipos de sessões incluem áudio e vídeo. |


