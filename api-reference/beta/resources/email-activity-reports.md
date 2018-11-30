---
title: Relatórios de atividades do email
description: Você pode obter um modo de exibição de alto nível de tráfego de email dentro da sua organização a partir da página de relatórios. Você também pode analisar o widget da atividade de Email para entender as tendências e detalhes por usuário da atividade de email na sua organização.
ms.openlocfilehash: 47ff9017216fa3fd333b383f7a603354775d1023
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041056"
---
# <a name="email-activity-reports"></a>Relatórios de atividades do email

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode obter um modo de exibição de alto nível de tráfego de email dentro da sua organização a partir da página de relatórios. Você também pode analisar o widget da atividade de Email para entender as tendências e detalhes por usuário da atividade de email na sua organização.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getemailactivityuserdetail.md) | Fluxo          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | Obtenha dados sobre as atividades de email que os usuários realizaram. |
| [Obter contagens de atividade](../api/reportroot-getemailactivitycounts.md) | Fluxo          | [emailActivitySummary](../resources/emailactivitysummary.md) | Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização. |
| [Obter contagens de usuários](../api/reportroot-getemailactivityusercounts.md) | Fluxo          | [emailActivitySummary](../resources/emailactivitysummary.md) | Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber. |
