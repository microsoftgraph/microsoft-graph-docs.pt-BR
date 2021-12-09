---
title: Relatório de atividades do SharePoint
description: Você pode obter a atividade de cada usuário licenciado para usar SharePoint olhando para a interação deles com arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b1fe7edaea8e7d2d6cc5a0da83dc7fd739a77d6e
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391078"
---
# <a name="sharepoint-activity-reports"></a>Relatório de atividades do SharePoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter a atividade de cada usuário licenciado para usar SharePoint olhando para a interação deles com arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - SharePoint atividade](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter dados de usuário](../api/reportroot-getsharepointactivityuserdetail.md) | Fluxo          | Fluxo           | Obtenha dados sobre as atividades do SharePoint por usuário.               |
| [Obter contagens de arquivo](../api/reportroot-getsharepointactivityfilecounts.md) | Fluxo          | Fluxo           | Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint. |
| [Obter contagens de usuários](../api/reportroot-getsharepointactivityusercounts.md) | Fluxo          | Fluxo           | Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado. |
| [Obter páginas](../api/reportroot-getsharepointactivitypages.md) | Fluxo          | Fluxo           | Obtenha o número de páginas exclusivas visitadas pelos usuários.             |


