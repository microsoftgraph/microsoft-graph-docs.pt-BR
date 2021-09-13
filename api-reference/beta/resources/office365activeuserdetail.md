---
title: Tipo de recurso office365ActiveUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 9f41a0b1fa74c203bfe6b46e9d7ed9788ba46ff5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115132"
---
# <a name="office365activeuserdetail-resource-type"></a>Tipo de recurso office365ActiveUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo              | Descrição                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Data              | A data mais recente do conteúdo.          |
| userPrincipalName                 | String            | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. |
| displayName                       | String            | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. |
| isDeleted                         | Boleano           | Se esse usuário foi excluído ou excluído. |
| deletedDate                       | Data              | A data em que a operação de exclusão aconteceu. O valor padrão é "null" quando o usuário não foi excluído. |
| hasExchangeLicense                | Boleano           | Se o usuário recebeu uma licença de Exchange. |
| hasOneDriveLicense                | Boleano           | Se o usuário recebeu uma licença de OneDrive. |
| hasSharePointLicense              | Boleano           | Se o usuário recebeu uma licença de SharePoint. |
| hasSkypeForBusinessLicense        | Boleano           | Se o usuário recebeu uma licença Skype for Business. |
| hasYammerLicense                  | Boleano           | Se o usuário recebeu uma licença de Yammer. |
| hasTeamsLicense                   | Boleano           | Se o usuário recebeu uma licença de Teams. |
| exchangeLastActivityDate          | Data              | A data em que o usuário leu ou enviou emails pela última vez. |
| oneDriveLastActivityDate          | Data              | A data em que o usuário foi exibido pela última vez ou editou arquivos, arquivos compartilhados interna ou externamente ou arquivos sincronizados. |
| sharePointLastActivityDate        | Data              | A data em que o usuário foi exibido pela última vez ou editou arquivos, arquivos compartilhados interna ou externamente, arquivos sincronizados ou exibidos SharePoint páginas. |
| skypeForBusinessLastActivityDate  | Data              | A data em que o usuário organizou ou participou da última vez em conferências ou ingressou em sessões ponto a ponto. |
| yammerLastActivityDate            | Data              | A data em que o usuário postou pela última vez, leu ou gostou da mensagem. |
| teamsLastActivityDate             | Data              | A data em que o usuário postou pela última vez mensagens em canais de equipe, enviou mensagens em sessões de chat privadas ou participou de reuniões ou chamadas. |
| exchangeLicenseAssignDate         | Data              | A última data em que o usuário foi atribuído a uma Exchange de usuário. |
| oneDriveLicenseAssignDate         | Data              | A última data em que o usuário foi atribuído a uma OneDrive de usuário. |
| sharePointLicenseAssignDate       | Data              | A última data em que o usuário foi atribuído a uma SharePoint de usuário. |
| skypeForBusinessLicenseAssignDate | Data              | A última data em que o usuário foi atribuído a uma licença Skype for Business. |
| yammerLicenseAssignDate           | Data              | A última data em que o usuário foi atribuído a uma Yammer de usuário. |
| teamsLicenseAssignDate            | Data              | A última data em que o usuário foi atribuído a uma Teams de usuário. |
| assignedProducts                  | String collection | Todos os produtos atribuídos ao usuário.  |

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


