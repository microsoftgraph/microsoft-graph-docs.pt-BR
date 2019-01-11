---
title: Relatórios de atividades de grupos do Yammer
description: Você pode obter ideias para a atividade do Yammer grupos em sua organização e ver quantos grupos do Yammer estão sendo criadas e usadas.
localization_priority: Normal
ms.openlocfilehash: 90be4037871480b7d694f4f9089d5f62064c9d2b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890668"
---
# <a name="yammer-groups-activity-reports"></a>Relatórios de atividades de grupos do Yammer

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção. Essas APIs não são suportadas na China Microsoft Graph operado pela 21Vianet.

Você pode obter ideias para a atividade do Yammer grupos em sua organização e ver quantos grupos do Yammer estão sendo criadas e usadas.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade de grupos do Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de grupo](../api/reportroot-getyammergroupsactivitydetail.md) | Fluxo          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | Obtenha dados sobre as atividades de grupo do Yammer por grupo. |
| [Obter contagens de grupo](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Fluxo          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo. |
| [Obter contagens de atividade](../api/reportroot-getyammergroupsactivitycounts.md) | Fluxo          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer. |
