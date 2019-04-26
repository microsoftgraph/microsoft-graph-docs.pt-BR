---
title: Relatórios de atividades do Yammer
description: Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 792b639a2f843a0b902b3a153eee16da3c0b3b76
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342769"
---
# <a name="yammer-activity-reports"></a>Relatórios de atividades do Yammer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getyammeractivityuserdetail.md) | Fluxo          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | Obtenha dados sobre as atividades do Yammer por usuário. |
| [Obter contagens de atividade](../api/reportroot-getyammeractivitycounts.md) | Fluxo          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas. |
| [Obter contagens de usuários](../api/reportroot-getyammeractivityusercounts.md) | Fluxo          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Obtenha as tendências do número de usuários exclusivos que lançaram, ler e curtiram mensagens do Yammer. |
