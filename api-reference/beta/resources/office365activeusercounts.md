---
title: tipo de recurso office365ActiveUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 8d640bbb3f49c95902134893f1eba4b4064ccca5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092451"
---
# <a name="office365activeusercounts-resource-type"></a>tipo de recurso office365ActiveUserCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A última data do conteúdo.          |
| Office365         | Int64  | O número de usuários ativos no Microsoft 365. Esse número inclui todos os usuários ativos no Exchange, OneDrive, SharePoint, Skype for Business, Yammer e Microsoft Teams. Você pode encontrar a definição de usuário ativo para cada produto na respectiva descrição da propriedade. |
| câmbio          | Int64  | O número de usuários ativos no Exchange. Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo. |
| oneDrive          | Int64  | O número de usuários ativos no OneDrive. Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, ou arquivos sincronizados é considerado um usuário ativo. |
| Do        | Int64  | O número de usuários ativos no SharePoint. Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, arquivos sincronizados ou páginas do SharePoint exibidas é considerado um usuário ativo. |
| skypeForBusiness  | Int64  | O número de usuários ativos no Skype for Business. Qualquer usuário que organizou ou participou de conferências ou sessões ponto a ponto Unidas é considerado um usuário ativo. |
| Yammer            | Int64  | O número de usuários ativos no Yammer. Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo. |
| Teams             | Int64  | O número de usuários ativos no Microsoft Teams. Qualquer usuário que lançou mensagens em canais de equipe, mensagens enviadas em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo. |
| reportDate        | Data   | A data em que um número de usuários estava ativo. |
| reportPeriod      | Cadeia de caracteres | O número de dias que o relatório cobre.    |

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


