---
title: tipo de recurso de office365ActiveUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 95912e736459894a69f8e2e1a18c2aaf672a19a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035841"
---
# <a name="office365activeuserdetail-resource-type"></a>tipo de recurso de office365ActiveUserDetail

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo              | Descrição                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Data              | A última data do conteúdo.          |
| userPrincipalName                 | String            | O usuário nome principal (UPN) do usuário. O UPN é um nome de logon estilo Internet para o usuário com base na Internet padrão RFC 822. Por convenção, isso deve ser mapeada para o nome de email do usuário. O formato geral é alias@domain, onde o domínio deve estar presente na coleção de locatário de domínios verificados. Essa propriedade é obrigatória quando um usuário é criado. |
| displayName                       | String            | O nome exibido para o usuário no catálogo de endereços. Geralmente é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. |
| isDeleted                         | Booliano           | Se esse usuário tiver sido excluído ou suave excluído. |
| deletedDate                       | Data              | A data quando a operação de exclusão aconteceu. Valor padrão é "nulo" quando o usuário não foi excluído. |
| hasExchangeLicense                | Booliano           | Se o usuário tenha sido atribuído uma licença do Exchange. |
| hasOneDriveLicense                | Booliano           | Se o usuário tenha sido atribuído uma licença do OneDrive. |
| hasSharePointLicense              | Booliano           | Se o usuário tenha sido atribuído uma licença do SharePoint. |
| hasSkypeForBusinessLicense        | Booliano           | Se o usuário tenha sido atribuído uma licença do Skype para negócios. |
| hasYammerLicense                  | Booliano           | Se o usuário tenha sido atribuído uma licença do Yammer. |
| hasTeamsLicense                   | Booliano           | Se o usuário tenha sido atribuído uma licença de equipes. |
| exchangeLastActivityDate          | Data              | A data quando o usuário última leitura ou enviado um email. |
| oneDriveLastActivityDate          | Data              | A data quando o usuário última exibidos ou editados arquivos, arquivos compartilhados interna ou externamente ou sincronizados arquivos. |
| sharePointLastActivityDate        | Data              | A data quando o usuário última exibidos ou editados arquivos, shared arquivos internamente ou externamente, sincronizados arquivos ou exibidos páginas do SharePoint. |
| skypeForBusinessLastActivityDate  | Data              | A data quando usuário última organizados participou de conferências ou ingressou sessões ponto a ponto. |
| yammerLastActivityDate            | Data              | A data quando usuário última postados, ler ou curtidas a mensagem. |
| teamsLastActivityDate             | Data              | A data em que o usuário lançada última mensagens no canais de equipe, mensagens enviadas em sessões de bate-papo privado ou participou chamadas ou reuniões. |
| exchangeLicenseAssignDate         | Data              | A última data em que o usuário foi atribuído a uma licença do Exchange. |
| oneDriveLicenseAssignDate         | Data              | A última data em que o usuário foi atribuído a uma licença do OneDrive. |
| sharePointLicenseAssignDate       | Data              | A última data em que o usuário foi atribuído a uma licença do SharePoint. |
| skypeForBusinessLicenseAssignDate | Data              | A última data em que o usuário foi atribuído a uma licença do Skype para negócios. |
| yammerLicenseAssignDate           | Data              | A última data em que o usuário foi atribuído a uma licença do Yammer. |
| teamsLicenseAssignDate            | Data              | A última data em que o usuário foi atribuído a uma licença de equipes. |
| assignedProducts                  | String collection | Todos os produtos atribuídos para o usuário.  |

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
