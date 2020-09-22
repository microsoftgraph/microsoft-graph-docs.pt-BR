---
title: tipo de recurso office365ActiveUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 05a47c175e7e9ed6334e691f91556190e459eec0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092416"
---
# <a name="office365activeuserdetail-resource-type"></a>tipo de recurso office365ActiveUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo              | Descrição                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Data              | A última data do conteúdo.          |
| userPrincipalName                 | String            | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. |
| displayName                       | String            | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. |
| isDeleted                         | Boolean           | Se este usuário foi excluído ou excluído por software. |
| deletedDate                       | Data              | A data em que a operação de exclusão ocorreu. O valor padrão é "nulo" quando o usuário não foi excluído. |
| hasExchangeLicense                | Boolean           | Se o usuário foi atribuído a uma licença do Exchange. |
| hasOneDriveLicense                | Boolean           | Se o usuário foi atribuído a uma licença do OneDrive. |
| hasSharePointLicense              | Boolean           | Se o usuário foi atribuído a uma licença do SharePoint. |
| hasSkypeForBusinessLicense        | Boolean           | Se o usuário foi atribuído a uma licença do Skype for Business. |
| hasYammerLicense                  | Boolean           | Se o usuário foi atribuído a uma licença do Yammer. |
| hasTeamsLicense                   | Boolean           | Se o usuário foi atribuído a uma licença do teams. |
| exchangeLastActivityDate          | Data              | A data em que o usuário leu ou enviou email pela última vez. |
| oneDriveLastActivityDate          | Data              | A data em que o usuário exibiu ou editou arquivos, arquivos compartilhados internamente ou externamente, ou arquivos sincronizados. |
| sharePointLastActivityDate        | Data              | A data em que o usuário exibiu ou editou arquivos, arquivos compartilhados internamente ou externamente, arquivos sincronizados ou páginas do SharePoint visualizadas por último. |
| skypeForBusinessLastActivityDate  | Data              | A data em que o usuário organizou ou participou de conferências ou sessões ponto a ponto Unidas. |
| yammerLastActivityDate            | Data              | A data em que o usuário postou, leu ou curtiu a mensagem. |
| teamsLastActivityDate             | Data              | A data em que o usuário postou mensagens em canais de equipe, enviou mensagens em sessões de chat privadas ou participou de reuniões ou chamadas. |
| exchangeLicenseAssignDate         | Data              | A última data em que o usuário recebeu uma licença do Exchange. |
| oneDriveLicenseAssignDate         | Data              | A última data em que o usuário recebeu uma licença do OneDrive. |
| sharePointLicenseAssignDate       | Data              | A última data em que o usuário recebeu uma licença do SharePoint. |
| skypeForBusinessLicenseAssignDate | Data              | A última data em que o usuário recebeu uma licença do Skype for Business. |
| yammerLicenseAssignDate           | Data              | A última data em que o usuário recebeu uma licença do Yammer. |
| teamsLicenseAssignDate            | Data              | A última data em que o usuário recebeu uma licença do teams. |
| assignedProducts                  | Coleção String | Todos os produtos atribuídos para o usuário.  |

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


