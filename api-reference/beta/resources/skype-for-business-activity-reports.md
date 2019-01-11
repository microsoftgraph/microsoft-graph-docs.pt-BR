---
title: Relatórios de atividades do Skype for Business
description: Você pode obter detalhes sobre a atividade em toda a organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.
localization_priority: Normal
ms.openlocfilehash: f27efa2b07345d73ef0a5b0034aca4f0f3e25793
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891620"
---
# <a name="skype-for-business-activity-reports"></a>Relatórios de atividades do Skype for Business

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode obter detalhes sobre a atividade em toda a organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Fluxo          | [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) | Obtenha dados sobre a atividade do Skype for Business por usuário. |
| [Obter contagens de atividade](../api/reportroot-getskypeforbusinessactivitycounts.md) | Fluxo          | [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) | Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Fluxo          | [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) | Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto. |
