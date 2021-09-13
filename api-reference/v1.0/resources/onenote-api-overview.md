---
title: Usar o API REST do OneNote
description: O Microsoft Graph permite que seu aplicativo obtenha acesso autorizado aos blocos de anotações, seções e páginas do OneNote de um usuário em uma conta pessoal ou de organização. Com as permissões delegadas ou de aplicativo apropriadas, seu aplicativo pode acessar os dados do OneNote do usuário conectado ou de qualquer usuário em um locatário.
ms.localizationpriority: high
author: jewan-microsoft
ms.prod: onenote
doc_type: conceptualPageType
ms.openlocfilehash: 9d34da129e354134a55efb682c5be098c73baaad
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094181"
---
# <a name="use-the-onenote-rest-api"></a>Usar o API REST do OneNote

O Microsoft Graph permite que seu aplicativo obtenha acesso autorizado aos blocos de anotações, seções e páginas de um usuário do OneNote em uma conta pessoal ou organizacional. Com as [permissões delegadas ou de aplicativo apropriadas](/graph/permissions-reference#notes-permissions), seu aplicativo pode acessar os dados do OneNote do usuário conectado ou de qualquer usuário em um locatário.

## <a name="root-url"></a>URL raiz
A URL raiz de serviço do OneNote usa o formato a seguir para todas as chamadas da API do OneNote.
```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar:

- `v1.0` serve para o código de produção estável.
- `beta` é experimentar um recurso que está em desenvolvimento. Os recursos e a funcionalidade do ponto de extremidade beta podem alterar; não recomendamos que você o use em seu código de produção.

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
- `users/{id}` é para conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual. Use a API de [usuários](users.md).
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

