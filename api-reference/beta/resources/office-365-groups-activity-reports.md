---
title: Relatórios de atividades do Microsoft 365 groups
description: Você pode obter informações sobre a atividade de grupos do Microsoft 365 em sua organização e ver quantos grupos da Microsoft 365 estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0b2a4fbb3a95f816ef730bcc16f2742a70160de0
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896809"
---
# <a name="microsoft-365-groups-activity-reports"></a>Relatórios de atividades do Microsoft 365 groups

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter informações sobre a atividade de grupos do Microsoft 365 em sua organização e ver quantos grupos da Microsoft 365 estão sendo criados e usados.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | Obtenha detalhes sobre a atividade de grupos do Microsoft 365 por grupo. |
| [Obter contagens de atividade](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo. |
| [Obter contagens de grupo](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint. |
| [Obter armazenamento](../api/reportroot-getoffice365groupsactivitystorage.md) | Fluxo          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo. |
| [Obter contagens de arquivo](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Fluxo          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites de grupo associados a um grupo do Microsoft 365. |
