---
title: Tipo de recurso office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: fe2df5614525f27b294bed93be7f3f9cd8170b30
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981505"
---
# <a name="office365groupsactivitydetail-resource-type"></a>Tipo de recurso office365GroupsActivityDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo    | Descrição                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | Cadeia de caracteres  | A ID do grupo.          |
| reportRefreshDate                 | Data    | A última data do conteúdo.          |
| groupDisplayName                  | Cadeia de caracteres  | O nome de exibição do grupo.           |
| isDeleted                         | Booliano | Se esse usuário foi excluído ou excluído de forma suave. |
| ownerPrincipalName                | Cadeia de caracteres  | O nome principal do proprietário do grupo.          |
| lastActivityDate                  | Data    | A data da última atividade para os seguintes cenários: caixa de correio de grupo recebeu emails; usuário visualizado, editado, compartilhado ou sincronizado arquivos na biblioteca de documentos do SharePoint; usuário visualizou páginas do SharePoint; usuário postou, leu ou curtiu mensagens em grupos do Yammer. |
| groupType                         | Cadeia de caracteres  | O tipo de grupo. Os valores possíveis são: **Public** ou **Private**. |
| memberCount                       | Int64   | A contagem de membros do grupo.                  |
| externalMemberCount               | Int64   | A contagem de membros externos do grupo.         |
| exchangeReceivedEmailCount        | Int64   | O número de emails que a caixa de correio do grupo recebeu. |
| sharePointActiveFileCount         | Int64   | O número de arquivos ativos no site do Grupo do SharePoint. |
| yammerPostedMessageCount          | Int64   | O número de mensagens postadas em grupos do Yammer. |
| yammerReadMessageCount            | Int64   | O número de mensagens lidas em grupos do Yammer. |
| yammerLikedMessageCount           | Int64   | O número de mensagens curtidas em grupos do Yammer. |
| exchangeMailboxTotalItemCount     | Int64   | O número de itens na caixa de correio do grupo. |
| exchangeMailboxStorageUsedInBytes | Int64   | O armazenamento usado da caixa de correio do grupo.   |
| sharePointTotalFileCount          | Int64   | O número total de arquivos no site do Grupo do SharePoint. |
| sharePointSiteStorageUsedInBytes  | Int64   | O armazenamento usado pelo site do Grupo do SharePoint. |
| reportPeriod                      | Cadeia de caracteres  | O número de dias que o relatório abrange.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```


