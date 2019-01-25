---
title: Relatórios dos usuários ativos do Office 365
description: Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças do produto estão sendo usadas por indivíduos em sua organização e fazer uma busca detalhada para obter informações sobre quais usuários estão usando quais produtos. Este relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e85924b7066dde92f0db5fd0b3f1f83dd32fd0c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516207"
---
# <a name="office-365-active-users-reports"></a>Relatórios dos usuários ativos do Office 365

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o relatório de usuários ativos do Office 365 para descobrir quantas licenças do produto estão sendo usadas por indivíduos em sua organização e fazer uma busca detalhada para obter informações sobre quais usuários estão usando quais produtos. Este relatório pode ajudar os administradores a identificar produtos subutilizados ou usuários que possam precisar de informações ou treinamento adicional.

> **Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Relatórios
| Função                                 | Tipo de retorno de CSV | Tipo de retorno JSON                         | Descrição                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Obter dados de usuário](../api/reportroot-getoffice365activeuserdetail.md) | Stream          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Obtenha dados sobre os usuários ativos do Office 365. |
| [Obter contagens de usuários](../api/reportroot-getoffice365activeusercounts.md) | Stream          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | Obtenha a contagem de usuários ativos diários no período de relatório por produto. |
| [Obter contagens de usuários dos serviços](../api/reportroot-getoffice365servicesusercounts.md) | Fluxo          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | Obtenha a contagem de usuários por tipo de atividade e serviço. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
