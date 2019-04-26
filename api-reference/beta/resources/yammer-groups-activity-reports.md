---
title: Relatórios de atividades de grupos do Yammer
description: Você pode obter informações sobre a atividade de grupos do yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9035984cf33c56811dc411a6c9cc01e6d438d194
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342785"
---
# <a name="yammer-groups-activity-reports"></a>Relatórios de atividades de grupos do Yammer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter informações sobre a atividade de grupos do yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getyammergroupsactivitydetail.md) | Fluxo          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | Obtenha dados sobre as atividades de grupo do Yammer por grupo. |
| [Obter contagens de grupo](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Fluxo          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo. |
| [Obter contagens de atividade](../api/reportroot-getyammergroupsactivitycounts.md) | Fluxo          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer. |
