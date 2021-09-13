---
title: Tipo de recurso office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 57d51cf3f2d4f91270000618a18f70f3804208c3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142863"
---
# <a name="office365groupsactivitydetail-resource-type"></a>Tipo de recurso office365GroupsActivityDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo    | Descrição                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | Cadeia de caracteres  | A ID do grupo.          |
| reportRefreshDate                 | Data    | A data mais recente do conteúdo.          |
| groupDisplayName                  | Cadeia de Caracteres  | O nome de exibição do grupo.           |
| isDeleted                         | Boleano | Se esse usuário foi excluído ou excluído. |
| ownerPrincipalName                | Cadeia de Caracteres  | O nome principal do proprietário do grupo.          |
| lastActivityDate                  | Data    | A última data de atividade para os seguintes cenários: caixa de correio de grupo recebeu emails; arquivos exibidos, editados, compartilhados ou sincronizados no SharePoint de documentos; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups. |
| groupType                         | Cadeia de Caracteres  | O tipo de grupo. Os valores possíveis são: **Público** ou **Privado**. |
| memberCount                       | Int64   | A contagem de membros do grupo.                  |
| externalMemberCount               | Int64   | A contagem de membros externos do grupo.         |
| exchangeReceivedEmailCount        | Int64   | O número de emails recebidos pela caixa de correio do grupo. |
| sharePointActiveFileCount         | Int64   | O número de arquivos ativos no site SharePoint Group. |
| yammerPostedMessageCount          | Int64   | O número de mensagens postadas em Yammer grupos. |
| yammerReadMessageCount            | Int64   | O número de mensagens lidas em Yammer grupos. |
| yammerLikedMessageCount           | Int64   | O número de mensagens curtidas em Yammer grupos. |
| exchangeMailboxTotalItemCount     | Int64   | O número de itens na caixa de correio do grupo. |
| exchangeMailboxStorageUsedInBytes | Int64   | O armazenamento usado da caixa de correio do grupo.   |
| sharePointTotalFileCount          | Int64   | O número total de arquivos no site SharePoint Group. |
| sharePointSiteStorageUsedInBytes  | Int64   | O armazenamento usado pelo site SharePoint Group. |
| reportPeriod                      | Cadeia de Caracteres  | O número de dias que o relatório aborda.    |

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


