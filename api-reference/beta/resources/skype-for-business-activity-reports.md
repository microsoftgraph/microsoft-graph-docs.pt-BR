---
title: Relatórios de atividades do Skype for Business
description: Você pode obter detalhes sobre a atividade em sua organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 965cf8b3c854360ea0b01f52e10e9241fd212d80
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897810"
---
# <a name="skype-for-business-activity-reports"></a>Relatórios de atividades do Skype for Business

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter detalhes sobre a atividade em sua organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.

> **Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Skype for Business Activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) | Obtenha dados sobre a atividade do Skype for Business por usuário. |
| [Obter contagens de atividade](../api/reportroot-getskypeforbusinessactivitycounts.md) | Fluxo          | [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) | Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Fluxo          | [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) | Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto. |
