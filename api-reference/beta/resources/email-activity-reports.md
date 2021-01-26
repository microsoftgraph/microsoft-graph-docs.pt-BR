---
title: Relatórios de atividades do email
description: Você pode obter uma visão de alto nível do tráfego de email em sua organização na página Relatórios. Você também pode detalhar o widget Atividade de Email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.
localization_priority: Normal
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: db9ea032b418a6beca7afb7c15eb16b762e6ed11
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983794"
---
# <a name="email-activity-reports"></a>Relatórios de atividades do email

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter uma visão de alto nível do tráfego de email em sua organização na página Relatórios. Você também pode detalhar o widget Atividade de Email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.

> **Observação:** Para saber mais sobre os diferentes modos de exibição de relatório e nomes, confira [Relatórios do Microsoft 365 - Atividade de E-mail](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getemailactivityuserdetail.md) | Fluxo          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | Obtenha dados sobre as atividades de email que os usuários realizaram. |
| [Obter contagens de atividade](../api/reportroot-getemailactivitycounts.md) | Fluxo          | [emailActivitySummary](../resources/emailactivitysummary.md) | Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização. |
| [Obter contagens de usuários](../api/reportroot-getemailactivityusercounts.md) | Fluxo          | [emailActivitySummary](../resources/emailactivitysummary.md) | Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber. |


