---
title: Tipo de recurso office365ActiveUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 057490d5e19a8e56a2e83047277292fbd0af4a16
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980686"
---
# <a name="office365activeuserdetail-resource-type"></a>Tipo de recurso office365ActiveUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo              | Descrição                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Data              | A data mais recente do conteúdo.          |
| userPrincipalName                 | String            | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. |
| displayName                       | String            | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. |
| isDeleted                         | Booliano           | Se esse usuário foi excluído ou excluído de forma suave. |
| deletedDate                       | Data              | A data em que a operação de exclusão ocorreu. O valor padrão é "null" quando o usuário não foi excluído. |
| hasExchangeLicense                | Booliano           | Se o usuário recebeu uma licença do Exchange. |
| hasOneDriveLicense                | Booliano           | Se o usuário recebeu uma licença do OneDrive. |
| hasSharePointLicense              | Booliano           | Se o usuário recebeu uma licença do SharePoint. |
| hasSkypeForBusinessLicense        | Booliano           | Se o usuário recebeu uma licença do Skype for Business. |
| hasYammerLicense                  | Booliano           | Se o usuário recebeu uma licença do Yammer. |
| hasTeamsLicense                   | Booliano           | Se o usuário recebeu uma licença do Teams. |
| exchangeLastActivityDate          | Data              | A data em que o usuário leu ou enviou emails pela última vez. |
| oneDriveLastActivityDate          | Data              | A data em que o usuário visualizou ou editou arquivos pela última vez, arquivos compartilhados interna ou externamente ou arquivos sincronizados. |
| sharePointLastActivityDate        | Data              | A data em que o usuário visualizou ou editou arquivos pela última vez, arquivos compartilhados interna ou externamente, arquivos sincronizados ou páginas do SharePoint exibidas pela última vez. |
| skypeForBusinessLastActivityDate  | Data              | A data em que o usuário organizou ou participou pela última vez em conferências, ou sessões ponto a ponto ingressadas. |
| yammerLastActivityDate            | Data              | A data em que o usuário postou, leu ou curtiu a mensagem pela última vez. |
| teamsLastActivityDate             | Data              | A data em que o usuário publicou pela última vez mensagens em canais de equipe, enviou mensagens em sessões de chat particular ou participou de reuniões ou chamadas. |
| exchangeLicenseAssignDate         | Data              | A última data em que o usuário foi atribuído com uma licença do Exchange. |
| oneDriveLicenseAssignDate         | Data              | A última data em que o usuário foi atribuído com uma licença do OneDrive. |
| sharePointLicenseAssignDate       | Data              | A última data em que o usuário foi atribuído a uma licença do SharePoint. |
| skypeForBusinessLicenseAssignDate | Data              | A última data em que o usuário foi atribuído com uma licença do Skype for Business. |
| yammerLicenseAssignDate           | Data              | A última data em que o usuário foi atribuído a uma licença do Yammer. |
| teamsLicenseAssignDate            | Data              | A última data em que o usuário foi atribuído com uma licença do Teams. |
| assignedProducts                  | Coleção String | Todos os produtos atribuídos ao usuário.  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "hasExchangeLicense": true, 
  "hasOneDriveLicense": true, 
  "hasSharePointLicense": true, 
  "hasSkypeForBusinessLicense": true, 
  "hasYammerLicense": true, 
  "hasTeamsLicense": true, 
  "exchangeLastActivityDate": "Date", 
  "oneDriveLastActivityDate": "Date", 
  "sharePointLastActivityDate": "Date", 
  "skypeForBusinessLastActivityDate": "Date", 
  "yammerLastActivityDate": "Date", 
  "teamsLastActivityDate": "Date", 
  "exchangeLicenseAssignDate": "Date", 
  "oneDriveLicenseAssignDate": "Date", 
  "sharePointLicenseAssignDate": "Date", 
  "skypeForBusinessLicenseAssignDate": "Date", 
  "yammerLicenseAssignDate": "Date", 
  "teamsLicenseAssignDate": "Date", 
  "assignedProducts": ["String"]
}
```


