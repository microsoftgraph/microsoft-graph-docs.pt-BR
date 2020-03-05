---
title: tipo de recurso office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: d517763fdfcbf046c36fc944d229b9a15b0cb8fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522446"
---
# <a name="office365groupsactivitydetail-resource-type"></a>tipo de recurso office365GroupsActivityDetail

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo    | Descrição                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| groupId                           | Cadeia de caracteres  | A ID do grupo.          |
| reportRefreshDate                 | Data    | A última data do conteúdo.          |
| groupDisplayName                  | String  | O nome de exibição do grupo.           |
| isDeleted                         | Boolean | Se este usuário foi excluído ou excluído por software. |
| ownerPrincipalName                | String  | O nome principal do proprietário do grupo.          |
| lastActivityDate                  | Data    | A data da última atividade dos seguintes cenários: caixa de correio de grupo recebidas emails; arquivos de usuário exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint; páginas do SharePoint exibidas pelo usuário; mensagens postadas, lidas ou curtidas pelo usuário em grupos do Yammer. |
| groupType                         | String  | O tipo de grupo. Os valores possíveis são: **Public** ou **Private**. |
| memberCount                       | Int64   | A contagem de membros do grupo.                  |
| externalMemberCount               | Int64   | A contagem de membros externos de grupo.         |
| exchangeReceivedEmailCount        | Int64   | O número de emails que a caixa de correio de grupo recebeu. |
| sharePointActiveFileCount         | Int64   | O número de arquivos ativos no site de grupo do SharePoint. |
| yammerPostedMessageCount          | Int64   | O número de mensagens postadas nos grupos do Yammer. |
| yammerReadMessageCount            | Int64   | O número de mensagens lidas nos grupos do Yammer. |
| yammerLikedMessageCount           | Int64   | O número de mensagens curtidas em grupos do Yammer. |
| exchangeMailboxTotalItemCount     | Int64   | O número de itens na caixa de correio do grupo. |
| exchangeMailboxStorageUsedInBytes | Int64   | O armazenamento usado da caixa de correio do grupo.   |
| sharePointTotalFileCount          | Int64   | O número total de arquivos no site de grupo do SharePoint. |
| sharePointSiteStorageUsedInBytes  | Int64   | O armazenamento usado pelo site de grupo do SharePoint. |
| reportPeriod                      | String  | O número de dias que o relatório cobre.    |

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
