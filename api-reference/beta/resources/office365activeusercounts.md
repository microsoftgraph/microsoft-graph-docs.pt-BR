---
title: Tipo de recurso office365ActiveUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 2f11c81394dd346d46b50d2c9a19eefb56984956
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026760"
---
# <a name="office365activeusercounts-resource-type"></a>Tipo de recurso office365ActiveUserCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A data mais recente do conteúdo.          |
| office365         | Int64  | O número de usuários ativos Microsoft 365. Esse número inclui todos os usuários ativos em Exchange, OneDrive, SharePoint, Skype For Business, Yammer e Microsoft Teams. Você pode encontrar a definição de usuário ativo para cada produto na descrição da respectiva propriedade. |
| exchange          | Int64  | O número de usuários ativos Exchange. Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo. |
| oneDrive          | Int64  | O número de usuários ativos OneDrive. Qualquer usuário que visualizou ou editou arquivos, arquivos compartilhados interna ou externamente ou arquivos sincronizados é considerado um usuário ativo. |
| sharePoint        | Int64  | O número de usuários ativos SharePoint. Qualquer usuário que visualizou ou editou arquivos, compartilhou arquivos interna ou externamente, arquivos sincronizados ou SharePoint páginas exibidas é considerado um usuário ativo. |
| skypeForBusiness  | Int64  | O número de usuários ativos no Skype For Business. Qualquer usuário que organizou ou participou de conferências ou ingressou em sessões ponto a ponto é considerado um usuário ativo. |
| yammer            | Int64  | O número de usuários ativos Yammer. Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo. |
| teams             | Int64  | O número de usuários ativos Microsoft Teams. Qualquer usuário que postou mensagens em canais de equipe, enviou mensagens em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo. |
| reportDate        | Data   | A data em que vários usuários estavam ativos. |
| reportPeriod      | Cadeia de caracteres | O número de dias que o relatório aborda.    |

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


