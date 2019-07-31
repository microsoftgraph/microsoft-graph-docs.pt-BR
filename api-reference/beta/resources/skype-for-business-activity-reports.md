---
title: Relatórios de atividades do Skype for Business
description: Você pode obter detalhes sobre a atividade em sua organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: fcd23201732f1e0988853ae33cf08a24295a2647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008240"
---
# <a name="skype-for-business-activity-reports"></a>Relatórios de atividades do Skype for Business

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter detalhes sobre a atividade em sua organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Fluxo          | [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) | Obtenha dados sobre a atividade do Skype for Business por usuário. |
| [Obter contagens de atividade](../api/reportroot-getskypeforbusinessactivitycounts.md) | Fluxo          | [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) | Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Fluxo          | [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) | Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto. |
