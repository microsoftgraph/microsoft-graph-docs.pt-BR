---
title: Relatórios de atividades do Yammer
description: Você pode entender o nível de envolvimento da sua organização com o Yammer pela quantidade de atividade gerada em toda a organização e pelo número de usuários exclusivos que postam, gostam e leem mensagens no Yammer.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: c0009949b5eb429f15155059768365b201078134
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982464"
---
# <a name="yammer-activity-reports"></a>Relatórios de atividades do Yammer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode entender o nível de envolvimento da sua organização com o Yammer pela quantidade de atividade gerada em toda a organização e pelo número de usuários exclusivos que postam, gostam e leem mensagens no Yammer.

> **Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira [relatórios do Microsoft 365 - Atividade do Yammer.](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getyammeractivityuserdetail.md) | Fluxo          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | Obtenha dados sobre as atividades do Yammer por usuário. |
| [Obter contagens de atividades](../api/reportroot-getyammeractivitycounts.md) | Fluxo          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas. |
| [Obter contagens de usuários](../api/reportroot-getyammeractivityusercounts.md) | Fluxo          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Veja as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer. |


