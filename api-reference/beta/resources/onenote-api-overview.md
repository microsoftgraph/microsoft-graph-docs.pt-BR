---
title: Usar o API REST do OneNote
description: 'O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado às sessões, páginas e blocos de notas do usuário do OneNote em uma conta pessoal ou da organização. Com as permissões delegadas ou permissões de aplicativo apropriadas, seu aplicativo pode acessar dados do OneNote do usuário conectado ou de todos os usuários em um locatário. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: conceptualPageType
ms.openlocfilehash: 4f9c05d1e7bf8e652d740aff80704e24b5788a01
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039234"
---
# <a name="use-the-onenote-rest-api"></a>Usar o API REST do OneNote

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado às sessões, páginas e blocos de notas do usuário do OneNote em uma conta pessoal ou da organização. Com as [permissões delegadas ou permissões de aplicativo apropriadas](/graph/permissions-reference#notes-permissions) seu aplicativo pode acessar dados do OneNote do usuário conectado ou de todos os usuários em um locatário. 

## <a name="root-url"></a>URL raiz
A URL raiz de serviço do OneNote usa o formato a seguir para todas as chamadas da API do OneNote.

```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar:

- `v1.0` serve para o código de produção estável.
- `beta` serve para experimentar um recurso que está em desenvolvimento. Os recursos e funcionalidades na extremidade beta podem mudar; não recomendamos usá-lo no seu código de produção.

A localização pode ser blocos de anotações do usuário no Microsoft 365 ou no OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações hospedado no site de equipe do SharePoint no Microsoft 365. 

![Pilha de desenvolvimento da API do OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

## <a name="user-notebooks"></a>Blocos de anotações do usuário
Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).
- `users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual. Use a API de [usuários](users.md).
> **Observação:** Para obter as IDs de usuário, faça uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.

## <a name="group-notebooks"></a>Blocos de anotações de grupo

Para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="sharepoint-site-notebooks"></a>Blocos de anotações do SharePoint
Para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.


