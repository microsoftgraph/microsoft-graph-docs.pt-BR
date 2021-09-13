---
title: Microsoft 365 de atividades de grupos
description: Você pode usar os relatórios de atividades grupos para obter informações sobre a atividade de Microsoft 365 grupos em sua organização e ver quantos grupos de Microsoft 365 estão sendo criados e usados.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 487b8a6693a077f59fd3202c563a56fc8ffce0dc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084241"
---
# <a name="microsoft-365-groups-activity-reports"></a>Microsoft 365 de atividades de grupos

Namespace: microsoft.graph

Você pode usar os relatórios de atividades grupos para obter informações sobre a atividade de Microsoft 365 grupos em sua organização e ver quantos grupos de Microsoft 365 estão sendo criados e usados.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - Microsoft 365 grupos](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getoffice365groupsactivitydetail.md) | Fluxo          | Obter detalhes sobre Microsoft 365 grupos por grupo. |
| [Obter contagens de atividade](../api/reportroot-getoffice365groupsactivitycounts.md) | Fluxo          | Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo. |
| [Obter contagens de grupo](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Fluxo          | Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint. |
| [Obter armazenamento](../api/reportroot-getoffice365groupsactivitystorage.md) | Fluxo          | Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo. |
| [Obter contagens de arquivo](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Fluxo          | Obter o número total de arquivos e quantos deles estavam ativos em todos os sites de grupo associados a um Microsoft 365 grupo. |

