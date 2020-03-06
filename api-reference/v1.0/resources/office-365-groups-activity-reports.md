---
title: Relatórios de atividades dos Grupos do Office 365
description: Você pode usar os relatórios de atividades dos Grupos para obter informações sobre a atividade dos Grupos do Office 365 em sua organização e ver quantos Grupos do Office 365 estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 57749ca15e4eaf4aad14f3f914426d861ea45eeb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534180"
---
# <a name="office-365-groups-activity-reports"></a>Relatórios de atividades dos Grupos do Office 365

Namespace: microsoft.graph

Você pode usar os relatórios de atividades dos Grupos para obter informações sobre a atividade dos Grupos do Office 365 em sua organização e ver quantos Grupos do Office 365 estão sendo criados e usados.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno | Descrição                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | Obtenha dados sobre as atividades dos Grupos do Office 365 por grupo. |
| [Obter contagens de atividades](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo. |
| [Obter contagens de grupo](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | Obtenha o número total diário de grupos e quantos deles estavam ativos com base em conversas de email, postagens do Yammer e atividades de arquivo do SharePoint. |
| [Obter armazenamento](../api/reportroot-getoffice365groupsactivitystorage.md) | Fluxo          | Obtenha o armazenamento total usado em todas as caixas de correio de grupo e sites de grupo. |
| [Obter contagens de arquivo](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Fluxo          | Obtenha o número total de arquivos e quantos deles estavam ativos em todos os sites do grupo associados a um Grupo do Office 365. |
