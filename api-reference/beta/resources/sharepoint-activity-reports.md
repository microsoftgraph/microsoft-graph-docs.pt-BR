---
title: Relatório de atividades do SharePoint
description: Você pode obter a atividade de cada usuário licenciado para usar o SharePoint analisando sua interação com os arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 2e7b834f9bd4e1a440f0fd5167679ce0074668cd
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983780"
---
# <a name="sharepoint-activity-reports"></a>Relatório de atividades do SharePoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter a atividade de cada usuário licenciado para usar o SharePoint analisando sua interação com os arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.

> **Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - Atividade do SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getsharepointactivityuserdetail.md) | Fluxo          | [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) | Obtenha dados sobre as atividades do SharePoint por usuário. |
| [Obter contagens de arquivo](../api/reportroot-getsharepointactivityfilecounts.md) | Fluxo          | [siteActivitySummary](../resources/siteactivitysummary.md) | Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint. |
| [Obter contagens de usuários](../api/reportroot-getsharepointactivityusercounts.md) | Fluxo          | [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) | Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado. |
| [Obter páginas](../api/reportroot-getsharepointactivitypages.md) | Fluxo          | [sharePointActivityPages](../resources/sharepointactivitypages.md) | Obtenha o número de páginas exclusivas visitadas pelos usuários. |


