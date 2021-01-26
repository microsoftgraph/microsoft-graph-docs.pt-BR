---
title: Relatórios de atividades de grupos do Microsoft 365
description: Você pode usar os relatórios de atividades de Grupos para obter informações sobre a atividade de grupos do Microsoft 365 em sua organização e ver quantos grupos do Microsoft 365 estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7470eff43c2c77a63206cf24e0484360bf3371b6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980994"
---
# <a name="microsoft-365-groups-activity-reports"></a>Relatórios de atividades de grupos do Microsoft 365

Namespace: microsoft.graph

Você pode usar os relatórios de atividades de Grupos para obter informações sobre a atividade de grupos do Microsoft 365 em sua organização e ver quantos grupos do Microsoft 365 estão sendo criados e usados.

> **Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - grupos do Microsoft 365.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getoffice365groupsactivitydetail.md) | Fluxo          | Obter detalhes sobre a atividade de grupos do Microsoft 365 por grupo. |
| [Obter contagens de atividades](../api/reportroot-getoffice365groupsactivitycounts.md) | Fluxo          | Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo. |
| [Obter contagens de grupo](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Fluxo          | Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint. |
| [Obter armazenamento](../api/reportroot-getoffice365groupsactivitystorage.md) | Fluxo          | Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo. |
| [Obter contagens de arquivo](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Fluxo          | Obter o número total de arquivos e quantos deles estavam ativos em todos os sites de grupo associados a um grupo do Microsoft 365. |

