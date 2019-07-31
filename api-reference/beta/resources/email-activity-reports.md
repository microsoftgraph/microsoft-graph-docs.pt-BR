---
title: Relatórios de atividades do email
description: Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios. Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 2540934b93a1047df5b19c4fe1b477ba30fd798c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972268"
---
# <a name="email-activity-reports"></a>Relatórios de atividades do email

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter uma visão de alto nível do tráfego de email em sua organização na página relatórios. Você também pode analisar o widget atividade de email para entender as tendências e os detalhes por usuário da atividade de email em sua organização.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getemailactivityuserdetail.md) | Fluxo          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | Obtenha dados sobre as atividades de email que os usuários realizaram. |
| [Obter contagens de atividade](../api/reportroot-getemailactivitycounts.md) | Fluxo          | [emailActivitySummary](../resources/emailactivitysummary.md) | Permite que você compreenda as tendências da atividade de email (como quantos foram enviados, lidos e recebidos) em sua organização. |
| [Obter contagens de usuários](../api/reportroot-getemailactivityusercounts.md) | Fluxo          | [emailActivitySummary](../resources/emailactivitysummary.md) | Permite que você compreenda as tendências do número de usuários únicos que estão executando atividades de email, como enviar, ler e receber. |
