---
title: Relatório de atividades do SharePoint
description: Você pode usar os relatórios de atividades do SharePoint para obter as atividades de cada usuário licenciado para usar o SharePoint examinando sua interação com arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 1985fc2b62a3dc18418bd62c1bba06970388b9ce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035602"
---
# <a name="sharepoint-activity-reports"></a>Relatório de atividades do SharePoint

Namespace: microsoft.graph

Você pode usar os relatórios de atividades do SharePoint para obter as atividades de cada usuário licenciado para usar o SharePoint examinando sua interação com arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - SharePoint atividade](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getsharepointactivityuserdetail.md) | Fluxo      | Obtenha dados sobre as atividades do SharePoint por usuário. |
| [Obter contagens de arquivo](../api/reportroot-getsharepointactivityfilecounts.md) | Fluxo      | Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint. |
| [Obter contagens de usuários](../api/reportroot-getsharepointactivityusercounts.md) | Fluxo      | Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado. |
| [Obter páginas](../api/reportroot-getsharepointactivitypages.md) | Fluxo      | Obtenha o número de páginas exclusivas visitadas pelos usuários. |

