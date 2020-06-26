---
title: Relatórios de atividades de grupos do Yammer
description: Você pode obter informações sobre a atividade de grupos do yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: cdeb94c9b5b687ab9584a236daaafb7c018a809c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897467"
---
# <a name="yammer-groups-activity-reports"></a>Relatórios de atividades de grupos do Yammer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter informações sobre a atividade de grupos do yammer em sua organização e ver quantos grupos do Yammer estão sendo criados e usados.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Yammer groups Activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | Obtenha dados sobre as atividades de grupo do Yammer por grupo. |
| [Obter contagens de grupo](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Fluxo          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo. |
| [Obter contagens de atividade](../api/reportroot-getyammergroupsactivitycounts.md) | Fluxo          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer. |
