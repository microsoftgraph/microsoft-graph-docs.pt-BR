---
title: tipo de recurso de office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: a849932d646be61f3cedec76ecdafdaca941baaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033917"
---
# <a name="office365groupsactivitydetail-resource-type"></a>tipo de recurso de office365GroupsActivityDetail

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo    | Descrição                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| reportRefreshDate                 | Data    | A última data do conteúdo.          |
| groupDisplayName                  | String  | O nome de exibição do grupo.           |
| isDeleted                         | Booliano | Se esse usuário tiver sido excluído ou suave excluído. |
| ownerPrincipalName                | String  | O nome de entidade do proprietário do grupo.          |
| lastActivityDate                  | Data    | A data da última atividade para os seguintes cenários: email da caixa de correio recebida; de grupo usuário exibido, editado, compartilhados ou sincronizados arquivos na biblioteca de documentos do SharePoint; usuário exibir páginas do SharePoint; usuário postados, ler ou curtidas mensagens no Yammer grupos. |
| groupType                         | String  | O tipo de grupo. Os valores possíveis são: **pública** ou **privada**. |
| memberCount                       | Int64   | A contagem de membro do grupo.                  |
| externalMemberCount               | Int64   | A contagem de externo membro do grupo.         |
| exchangeReceivedEmailCount        | Int64   | O número de email que recebeu a caixa de correio de grupo. |
| sharePointActiveFileCount         | Int64   | O número de arquivos ativos no site de grupo do SharePoint. |
| yammerPostedMessageCount          | Int64   | O número de mensagens postadas em grupos de Yammer. |
| yammerReadMessageCount            | Int64   | O número de mensagens lidas em grupos do Yammer. |
| yammerLikedMessageCount           | Int64   | O número de mensagens curtidas em grupos do Yammer. |
| exchangeMailboxTotalItemCount     | Int64   | O número de itens na caixa de correio de grupo. |
| exchangeMailboxStorageUsedInBytes | Int64   | O armazenamento utilizado da caixa de correio de grupo.   |
| sharePointTotalFileCount          | Int64   | O número total de arquivos no site de grupo do SharePoint. |
| sharePointSiteStorageUsedInBytes  | Int64   | O armazenamento usado pelo site do grupo do SharePoint. |
| reportPeriod                      | String  | O número de dias que abrange o relatório.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
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
