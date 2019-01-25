---
title: Relatórios de atividades do Skype for Business
description: Você pode obter detalhes sobre a atividade em toda a organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a81e27d58316cb415d6296b4f77519a3f2125643
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512392"
---
# <a name="skype-for-business-activity-reports"></a>Relatórios de atividades do Skype for Business

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter detalhes sobre a atividade em toda a organização. Esses dados podem ajudar a investigar, planejar e tomar outras decisões comerciais para sua organização.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) | Obtenha dados sobre a atividade do Skype for Business por usuário. |
| [Obter contagens de atividade](../api/reportroot-getskypeforbusinessactivitycounts.md) | Fluxo          | [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) | Obtenha as tendências de quantos usuários organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream          | [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) | Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
