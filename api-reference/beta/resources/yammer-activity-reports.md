---
title: Relatórios de atividades do Yammer
description: Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 8f1358c188b06953d7af180c2b7ad83b6183af35
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519054"
---
# <a name="yammer-activity-reports"></a>Relatórios de atividades do Yammer

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode entender o nível do compromisso da sua organização com o Yammer por quanta atividade é gerada na organização e o número de usuários exclusivos que postam, gostam e lêem mensagens no Yammer.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | Obtenha dados sobre as atividades do Yammer por usuário. |
| [Obter contagens de atividade](../api/reportroot-getyammeractivitycounts.md) | Fluxo          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas. |
| [Obter contagens de usuários](../api/reportroot-getyammeractivityusercounts.md) | Fluxo          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Obtenha as tendências do número de usuários exclusivos que lançaram, ler e curtiram mensagens do Yammer. |
