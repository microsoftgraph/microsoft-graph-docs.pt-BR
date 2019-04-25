---
title: Usar a API REST do OneNote
description: 'O Microsoft Graph permite que o aplicativo obtenha acesso autorizado aos blocos de anotações, seções e páginas do OneNote de um usuário em uma conta pessoal ou de organização. Com as permissões delegadas ou de aplicativo apropriadas, seu aplicativo pode acessar os dados do OneNote do usuário conectado ou de qualquer usuário em um locatário. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7db3024224dde7ee4c95d2e3840187709471cecd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566042"
---
# <a name="use-the-onenote-rest-api"></a>Usar a API REST do OneNote

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Graph permite que o aplicativo obtenha acesso autorizado aos blocos de anotações, seções e páginas do OneNote de um usuário em uma conta pessoal ou de organização. Com as [permissões delegadas ou de aplicativo apropriadas](/graph/permissions-reference#notes-permissions), seu aplicativo pode acessar os dados do OneNote do usuário conectado ou de qualquer usuário em um locatário. 

## <a name="root-url"></a>URL Raiz
A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para a API do OneNote.
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

O `version` segmento na URL representa a versão do Microsoft Graph que você deseja usar:

- `v1.0` serve para o código de produção estável.
- `beta` serve para experimentar um recurso que está em desenvolvimento. Recursos e funcionalidades no ponto de extremidade beta podem mudar; Não recomendamos que você o use em seu código de produção.

O local pode ser blocos de anotações do usuário no Office 365 ou no OneDrive do consumidor, nos blocos de anotações de grupo ou em blocos de anotações de equipe hospedados no site do SharePoint no Office 365. 

![Pilha de desenvolvimento da API do OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>Blocos de anotações do usuário
Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).
- `users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual. Use a API de [usuários](users.md) .
> **Observação:** Você pode obter IDs de usuário fazendo uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.

### <a name="group-notebooks"></a>Blocos de anotações de grupo

Para acessar blocos de anotações pertencentes a um grupo, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>Blocos de anotações do site do SharePoint
Para acessar blocos de anotações pertencentes a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
