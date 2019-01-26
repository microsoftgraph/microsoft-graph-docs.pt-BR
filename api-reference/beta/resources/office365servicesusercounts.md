---
title: tipo de recurso de office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573890"
---
# <a name="office365servicesusercounts-resource-type"></a>tipo de recurso de office365ServicesUserCounts

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo   | Descrição                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Data   | A última data do conteúdo.          |
| exchangeActive           | Int64  | O número de usuários ativos em Exchange. Qualquer usuário que pode ler e enviar emails é considerado um usuário ativo. |
| exchangeInactive         | Int64  | O número de usuários inativos no Exchange. |
| oneDriveActive           | Int64  | O número de usuários ativos em OneDrive. Qualquer usuário que são exibidos ou editados arquivos, arquivos compartilhados interna ou externamente ou sincronizados arquivos é considerado um usuário ativo. |
| oneDriveInactive         | Int64  | O número de usuários inativos no OneDrive. |
| sharePointActive         | Int64  | O número de usuários ativos no SharePoint. Qualquer usuário que exibidos ou editados arquivos, internamente de arquivos compartilhados ou sincronizados arquivos externamente ou exibidos páginas do SharePoint é considerado um usuário ativo. |
| sharePointInactive       | Int64  | O número de usuários inativos no SharePoint. |
| skypeForBusinessActive   | Int64  | O número de usuários ativos em Skype para negócios. Qualquer usuário que organizou participou de conferências ou ingressou sessões ponto a ponto é considerado um usuário ativo. |
| skypeForBusinessInactive | Int64  | O número de usuários inativos em Skype para negócios. |
| yammerActive             | Int64  | O número de usuários ativos no Yammer. Qualquer usuário que pode postar, ler ou like mensagens é considerado um usuário ativo. |
| yammerInactive           | Int64  | O número de usuários inativos no Yammer.  |
| teamsActive              | Int64  | O número de usuários ativos em Teams da Microsoft. Qualquer usuário que as mensagens postadas no canais de equipe, mensagens enviadas em sessões de bate-papo privado ou participou chamadas ou reuniões é considerado um usuário ativo. |
| teamsInactive            | Int64  | O número de usuários inativos no Microsoft Teams.     |
| office365Active          | Int64  | O número de usuários ativos no Office 365.   |
| office365Inactive        | Int64  | O número de usuários inativos no Office 365.     |
| reportPeriod             | String | O número de dias que abrange o relatório.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```
