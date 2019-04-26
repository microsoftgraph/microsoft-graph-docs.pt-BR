---
title: Relatório de atividades do SharePoint
description: Você pode obter a atividade de cada usuário licenciado para usar o SharePoint examinando sua interação com os arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: cfe8c698533b46d4edbbb724dc5fb993cc85cfdb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343158"
---
# <a name="sharepoint-activity-reports"></a>Relatório de atividades do SharePoint

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter a atividade de cada usuário licenciado para usar o SharePoint examinando sua interação com os arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getsharepointactivityuserdetail.md) | Fluxo          | [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) | Obtenha dados sobre as atividades do SharePoint por usuário. |
| [Obter contagens de arquivo](../api/reportroot-getsharepointactivityfilecounts.md) | Fluxo          | [siteActivitySummary](../resources/siteactivitysummary.md) | Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint. |
| [Obter contagens de usuários](../api/reportroot-getsharepointactivityusercounts.md) | Fluxo          | [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) | Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado. |
| [Obter páginas](../api/reportroot-getsharepointactivitypages.md) | Fluxo          | [sharePointActivityPages](../resources/sharepointactivitypages.md) | Obtenha o número de páginas exclusivas visitadas pelos usuários. |
