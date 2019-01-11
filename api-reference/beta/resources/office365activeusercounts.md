---
title: tipo de recurso de office365ActiveUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 887f9b08d7f46aac023fbd0f34e6174e5f422760
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882716"
---
# <a name="office365activeusercounts-resource-type"></a>tipo de recurso de office365ActiveUserCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A última data do conteúdo.          |
| office365         | Int64  | O número de usuários ativos no Office 365. Esse número inclui todos os usuários ativos no Exchange, OneDrive, SharePoint, Skype For Business, Yammer e Teams da Microsoft. Você pode encontrar a definição de usuário ativo para cada produto na descrição do respectivas propriedades. |
| Exchange          | Int64  | O número de usuários ativos no Exchange. Qualquer usuário que pode ler e enviar emails é considerado um usuário ativo. |
| oneDrive          | Int64  | O número de usuários ativos no OneDrive. Qualquer usuário que são exibidos ou editados arquivos, arquivos compartilhados interna ou externamente ou sincronizados arquivos é considerado um usuário ativo. |
| sharePoint        | Int64  | O número de usuários ativos no SharePoint. Qualquer usuário que exibidos ou editados arquivos, internamente de arquivos compartilhados ou sincronizados arquivos externamente ou exibidos páginas do SharePoint é considerado um usuário ativo. |
| skypeForBusiness  | Int64  | O número de usuários ativos em Skype para negócios. Qualquer usuário que organizou participou de conferências ou ingressou sessões ponto a ponto é considerado um usuário ativo. |
| Yammer            | Int64  | O número de usuários ativos no Yammer. Qualquer usuário que pode postar, ler ou like mensagens é considerado um usuário ativo. |
| equipes             | Int64  | O número de usuários ativos em Microsoft Teams. Qualquer usuário que as mensagens postadas no canais de equipe, mensagens enviadas em sessões de bate-papo privado ou participou chamadas ou reuniões é considerado um usuário ativo. |
| reportDate        | Data   | A data em que um número de usuários estava ativo. |
| reportPeriod      | Cadeia de caracteres | O número de dias que abrange o relatório.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
