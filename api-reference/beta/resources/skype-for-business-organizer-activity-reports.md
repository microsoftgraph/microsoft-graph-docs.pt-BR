---
title: Relatórios de atividades do organizador do Skype for Business
description: Você pode obter detalhes sobre a atividade de conferências organizada em toda a organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 706e9d88e52756ac8df4db8fd5c738a50d545e37
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514051"
---
# <a name="skype-for-business-organizer-activity-reports"></a>Relatórios de atividades do organizador do Skype for Business

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode obter detalhes sobre a atividade de conferências organizada em toda a organização. Esses dados são muito úteis quando você está investigando, planejando e tomando outras decisões comerciais para sua organização.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do organizador da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).

## <a name="reports"></a>Relatórios

| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter contagens de atividade](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | Stream          | [skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md) | Obtenha tendências de uso do número e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft. |
| [Obter contagens de usuários](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | Stream          | [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) | Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Os tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, Web, dial-in/out por terceiros, dial-in/out pela Microsoft. |
| [Obter contagens de minutos](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | Fluxo          | [skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) | Obtenha tendências de uso na duração em minutos e tipo de sessões de conferência realizadas e organizadas pelos usuários em sua organização. Tipos de sessões de conferência incluem áudio/vídeo e dial-in/out pela Microsoft. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-organizer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
