---
title: tipo de recurso office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0deb5eceb31ca3453c1cc5f29ae669f7053738c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522418"
---
# <a name="office365servicesusercounts-resource-type"></a>tipo de recurso office365ServicesUserCounts

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo   | Descrição                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Data   | A última data do conteúdo.          |
| exchangeActive           | Int64  | O número de usuários ativos no Exchange. Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo. |
| exchangeInactive         | Int64  | O número de usuários inativos no Exchange. |
| oneDriveActive           | Int64  | O número de usuários ativos no OneDrive. Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, ou arquivos sincronizados é considerado um usuário ativo. |
| oneDriveInactive         | Int64  | O número de usuários inativos no OneDrive. |
| sharePointActive         | Int64  | O número de usuários ativos no SharePoint. Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, arquivos sincronizados ou páginas do SharePoint exibidas é considerado um usuário ativo. |
| sharePointInactive       | Int64  | O número de usuários inativos no SharePoint. |
| skypeForBusinessActive   | Int64  | O número de usuários ativos no Skype for Business. Qualquer usuário que organizou ou participou de conferências ou sessões ponto a ponto Unidas é considerado um usuário ativo. |
| skypeForBusinessInactive | Int64  | O número de usuários inativos no Skype for Business. |
| yammerActive             | Int64  | O número de usuários ativos no Yammer. Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo. |
| yammerInactive           | Int64  | O número de usuários inativos no Yammer.  |
| teamsActive              | Int64  | O número de usuários ativos no Microsoft Teams. Qualquer usuário que lançou mensagens em canais de equipe, mensagens enviadas em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo. |
| teamsInactive            | Int64  | O número de usuários inativos no Microsoft Teams.     |
| office365Active          | Int64  | O número de usuários ativos no Office 365.   |
| office365Inactive        | Int64  | O número de usuários inativos no Office 365.     |
| reportPeriod             | String | O número de dias que o relatório cobre.    |

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
