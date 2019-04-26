---
title: Relatórios de atividades dos Grupos do Office 365
description: Você pode obter informações sobre a atividade dos grupos do Office 365 em sua organização e ver quantos grupos do Office 365 estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a46e1823acd63616f10ce2569a72a0099e390f93
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342006"
---
# <a name="office-365-groups-activity-reports"></a>Relatórios de atividades dos Grupos do Office 365

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter informações sobre a atividade dos grupos do Office 365 em sua organização e ver quantos grupos do Office 365 estão sendo criados e usados.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getoffice365groupsactivitydetail.md) | Fluxo          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo. |
| [Obter contagens de atividade](../api/reportroot-getoffice365groupsactivitycounts.md) | Fluxo          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo. |
| [Obter contagens de grupo](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Fluxo          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint. |
| [Obter armazenamento](../api/reportroot-getoffice365groupsactivitystorage.md) | Fluxo          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo. |
| [Obter contagens de arquivo](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Fluxo          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365. |
