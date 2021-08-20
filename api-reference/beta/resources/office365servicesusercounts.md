---
title: Tipo de recurso office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 5e243e77595e361e271a8ecde3c36ba82ed85ba4c404154f7b0947bba762f145
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229413"
---
# <a name="office365servicesusercounts-resource-type"></a>Tipo de recurso office365ServicesUserCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo   | Descrição                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Data   | A data mais recente do conteúdo.          |
| exchangeActive           | Int64  | O número de usuários ativos Exchange. Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo. |
| exchangeInactive         | Int64  | O número de usuários inativos no Exchange. |
| oneDriveActive           | Int64  | O número de usuários ativos OneDrive. Qualquer usuário que visualizou ou editou arquivos, arquivos compartilhados interna ou externamente ou arquivos sincronizados é considerado um usuário ativo. |
| oneDriveInactive         | Int64  | O número de usuários inativos no OneDrive. |
| sharePointActive         | Int64  | O número de usuários ativos SharePoint. Qualquer usuário que visualizou ou editou arquivos, compartilhou arquivos interna ou externamente, arquivos sincronizados ou SharePoint páginas exibidas é considerado um usuário ativo. |
| sharePointInactive       | Int64  | O número de usuários inativos no SharePoint. |
| skypeForBusinessActive   | Int64  | O número de usuários ativos no Skype For Business. Qualquer usuário que organizou ou participou de conferências ou ingressou em sessões ponto a ponto é considerado um usuário ativo. |
| skypeForBusinessInactive | Int64  | O número de usuários inativos no Skype For Business. |
| yammerActive             | Int64  | O número de usuários ativos Yammer. Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo. |
| yammerInactive           | Int64  | O número de usuários inativos no Yammer.  |
| teamsActive              | Int64  | O número de usuários ativos Microsoft Teams. Qualquer usuário que postou mensagens em canais de equipe, enviou mensagens em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo. |
| teamsInactive            | Int64  | O número de usuários inativos no Microsoft Teams.     |
| office365Active          | Int64  | O número de usuários ativos Microsoft 365.   |
| office365Inactive        | Int64  | O número de usuários inativos no Microsoft 365.     |
| reportPeriod             | Cadeia de caracteres | O número de dias que o relatório aborda.    |

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


