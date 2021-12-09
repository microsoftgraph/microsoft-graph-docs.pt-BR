---
title: Yammer de atividades de grupos
description: Você pode obter informações sobre a atividade Yammer grupos em sua organização e ver quantos grupos Yammer estão sendo criados e usados.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 6afb080020f5a9032f26a34c8b91433db2b8e034
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390652"
---
# <a name="yammer-groups-activity-reports"></a>Yammer de atividades de grupos

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter informações sobre a atividade Yammer grupos em sua organização e ver quantos grupos Yammer estão sendo criados e usados.

> **Observação:** Para obter detalhes sobre diferentes exibições de relatório e nomes, [consulte Microsoft 365 relatórios - atividade Yammer grupos](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).

## <a name="reports"></a>Relatórios

| Função                                                     | Tipo de retorno CSV | Tipo de retorno JSON | Descrição                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Obter dados de grupo](../api/reportroot-getyammergroupsactivitydetail.md) | Fluxo          | Stream           | Obtenha dados sobre as atividades de grupo do Yammer por grupo.           |
| [Obter contagens de grupo](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Fluxo          | Stream           | Obtenha o número total de grupos que existiam e quantos incluíam atividade de conversação em grupo. |
| [Obter contagens de atividade](../api/reportroot-getyammergroupsactivitycounts.md) | Fluxo          | Stream           | Obtenha o número de mensagens postadas, lidas e curtidas em grupos do Yammer. |


