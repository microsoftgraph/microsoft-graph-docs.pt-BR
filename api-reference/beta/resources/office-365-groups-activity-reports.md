---
title: Relatórios de atividades dos Grupos do Office 365
description: Você pode obter ideias para a atividade do Office 365 grupos em sua organização e ver quantos grupos do Office 365 estão sendo criadas e usadas.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8db142bcc7ae283df41dd6809ab97e81c996c10a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971183"
---
# <a name="office-365-groups-activity-reports"></a>Relatórios de atividades dos Grupos do Office 365

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode obter ideias para a atividade do Office 365 grupos em sua organização e ver quantos grupos do Office 365 estão sendo criadas e usadas.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getoffice365groupsactivitydetail.md) | Fluxo          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo. |
| [Obter contagens de atividade](../api/reportroot-getoffice365groupsactivitycounts.md) | Fluxo          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo. |
| [Obter contagens de grupo](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Fluxo          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint. |
| [Obter armazenamento](../api/reportroot-getoffice365groupsactivitystorage.md) | Fluxo          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo. |
| [Obter contagens de arquivo](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Fluxo          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365. |
