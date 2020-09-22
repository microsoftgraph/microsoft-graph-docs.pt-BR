---
title: Relatório de atividades do SharePoint
description: Você pode usar os relatórios de atividades do SharePoint para obter as atividades de cada usuário licenciado para usar o SharePoint examinando sua interação com arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 80723ffd868d4b936dadb5fcbebcf4f373d2a4de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009153"
---
# <a name="sharepoint-activity-reports"></a>Relatório de atividades do SharePoint

Namespace: microsoft.graph

Você pode usar os relatórios de atividades do SharePoint para obter as atividades de cada usuário licenciado para usar o SharePoint examinando sua interação com arquivos. Você também pode observar o nível de colaboração em andamento com base no número de arquivos compartilhados.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-SharePoint Activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getsharepointactivityuserdetail.md) | Fluxo      | Obtenha dados sobre as atividades do SharePoint por usuário. |
| [Obter contagens de arquivo](../api/reportroot-getsharepointactivityfilecounts.md) | Fluxo      | Obtenha o número de usuários únicos licenciados que interagiram com arquivos armazenados em sites do SharePoint. |
| [Obter contagens de usuários](../api/reportroot-getsharepointactivityusercounts.md) | Fluxo      | Obtenha a tendência no número de usuários ativos. Um usuário é considerado ativo se ele ou ela executou uma atividade de arquivo (salvar, sincronizar, modificar ou compartilhar) ou visitou uma página dentro do período de tempo especificado. |
| [Obter páginas](../api/reportroot-getsharepointactivitypages.md) | Fluxo      | Obtenha o número de páginas exclusivas visitadas pelos usuários. |

