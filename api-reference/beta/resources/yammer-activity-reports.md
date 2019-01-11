---
title: Relatórios de atividades do Yammer
description: Você pode compreender o nível de participação da sua organização com o Yammer por quanto atividade é gerada entre a organização e o número de usuários exclusivos que postar, like e ler mensagens no Yammer.
localization_priority: Normal
ms.openlocfilehash: 9895e37812b037b33f13682c3c56dacba5928d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823706"
---
# <a name="yammer-activity-reports"></a>Relatórios de atividades do Yammer

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção. Essas APIs não são suportadas na China Microsoft Graph operado pela 21Vianet.

Você pode compreender o nível de participação da sua organização com o Yammer por quanto atividade é gerada entre a organização e o número de usuários exclusivos que postar, like e ler mensagens no Yammer.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades do Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getyammeractivityuserdetail.md) | Fluxo          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | Obtenha dados sobre as atividades do Yammer por usuário. |
| [Obter contagens de atividade](../api/reportroot-getyammeractivitycounts.md) | Fluxo          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Obtenha as tendências da quantidade de atividade do Yammer em sua organização por quantas mensagens foram postadas, lidas e curtidas. |
| [Obter contagens de usuários](../api/reportroot-getyammeractivityusercounts.md) | Fluxo          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Obtenha as tendências do número de usuários exclusivos que postaram, leram e curtiram mensagens do Yammer. |
