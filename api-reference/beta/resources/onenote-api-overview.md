---
title: Usar a API REST do OneNote
description: 'O Microsoft Graph permite que o seu aplicativo obter acesso autorizado a um usuário OneNote blocos de anotações, seções e páginas em uma conta pessoal ou organização. Com o apropriado delegada ou permissões de aplicativo, seu aplicativo podem acessar os dados de OneNote do usuário conectado ou a qualquer usuário em um locatário. '
localization_priority: Normal
ms.openlocfilehash: 25817280fff570f0d87722fc8f3fadc9cf1c24d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815230"
---
# <a name="use-the-onenote-rest-api"></a>Usar a API REST do OneNote

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O Microsoft Graph permite que o seu aplicativo obter acesso autorizado a um usuário OneNote blocos de anotações, seções e páginas em uma conta pessoal ou organização. Com as [permissões apropriadas de delegada ou de aplicativos](/graph/permissions-reference#notes-permissions), seu aplicativo pode acessar os dados de OneNote do usuário conectado ou a qualquer usuário em um locatário. 

## <a name="root-url"></a>URL raiz
A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para o OneNote.
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

O `version` segmento na URL representa a versão do Microsoft Graph que você deseja usar:

- `v1.0` serve para o código de produção estável.
- `beta` serve para experimentar um recurso que está em desenvolvimento. Recursos e funcionalidades no ponto de extremidade beta podem ser alterado; não recomendamos que você usá-lo em seu código de produção.

O local pode ser blocos de anotações do usuário no Office 365 ou consumidor OneDrive, blocos de anotações do grupo ou blocos de anotações do SharePoint team site hospedado no Office 365. 

![Pilha do desenvolvimento de API do OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>Blocos de anotações do usuário
Para acessar os blocos de anotações pessoais consumidor OneDrive ou OneDrive for Business, use um dos seguintes URLs:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).
- `users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual. Use os [usuários](users.md) API.
> **Observação:** Você pode obter IDs de usuário fazendo uma solicitação GET na `https://graph.microsoft.com/v1.0/users`.

### <a name="group-notebooks"></a>Blocos de anotações do grupo

Para acessar os blocos de anotações pertencentes a um grupo, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>Blocos de anotações do site do SharePoint
Para acessar os blocos de anotações pertencentes a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
