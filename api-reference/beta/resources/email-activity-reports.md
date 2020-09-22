---
title: Relatórios de atividades do email
description: Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios. Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: f3c1ccd2700bce7a054cfec8fed943c01a3f4a1c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055544"
---
# <a name="email-activity-reports"></a>Relatórios de atividades do email

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios. Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-E-mail Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getemailactivityuserdetail.md) | Fluxo          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | Obtenha dados sobre as atividades de email que os usuários realizaram. |
| [Obter contagens de atividade](../api/reportroot-getemailactivitycounts.md) | Fluxo          | [emailActivitySummary](../resources/emailactivitysummary.md) | Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização. |
| [Obter contagens de usuários](../api/reportroot-getemailactivityusercounts.md) | Fluxo          | [emailActivitySummary](../resources/emailactivitysummary.md) | Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber. |


