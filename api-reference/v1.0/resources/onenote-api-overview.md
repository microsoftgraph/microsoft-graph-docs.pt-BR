---
title: Usar o API REST do OneNote
description: O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado às sessões, páginas e blocos de notas do usuário do OneNote em uma conta pessoal ou da organização. Com as permissões delegadas ou permissões de aplicativo apropriadas, seu aplicativo pode acessar dados do OneNote do usuário conectado ou de todos os usuários em um locatário.
localization_priority: Priority
author: jewan-microsoft
ms.prod: onenote
doc_type: conceptualPageType
ms.openlocfilehash: c22f38e7002e7619b1e9ee182866e850cf83cdf9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035914"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="93ea8-104">Usar o API REST do OneNote</span><span class="sxs-lookup"><span data-stu-id="93ea8-104">Use the OneNote REST API</span></span>

<span data-ttu-id="93ea8-105">O Microsoft Graph permite que o seu aplicativo obtenha acesso autorizado às sessões, páginas e blocos de notas do usuário do OneNote em uma conta pessoal ou da organização.</span><span class="sxs-lookup"><span data-stu-id="93ea8-105">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="93ea8-106">Com as [permissões delegadas ou permissões de aplicativo apropriadas](/graph/permissions-reference#notes-permissions) seu aplicativo pode acessar dados do OneNote do usuário conectado ou de todos os usuários em um locatário.</span><span class="sxs-lookup"><span data-stu-id="93ea8-106">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span>

## <a name="root-url"></a><span data-ttu-id="93ea8-107">URL raiz</span><span class="sxs-lookup"><span data-stu-id="93ea8-107">Root URL</span></span>
<span data-ttu-id="93ea8-108">A URL raiz de serviço do OneNote usa o formato a seguir para todas as chamadas da API do OneNote.</span><span class="sxs-lookup"><span data-stu-id="93ea8-108">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
<span data-ttu-id="93ea8-109">O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar:</span><span class="sxs-lookup"><span data-stu-id="93ea8-109">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="93ea8-110">`v1.0` serve para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="93ea8-110">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="93ea8-111">`beta` serve para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="93ea8-111">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="93ea8-112">Os recursos e funcionalidades na extremidade beta podem mudar; não recomendamos usá-lo no seu código de produção.</span><span class="sxs-lookup"><span data-stu-id="93ea8-112">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="93ea8-113">A localização pode ser blocos de anotações do usuário no Office 365 ou de consumidor do OneDrive, blocos de anotações de grupo ou blocos de anotações hospedado no site da equipe do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="93ea8-113">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![Pilha de desenvolvimento da API do OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="93ea8-115">Blocos de anotações do usuário</span><span class="sxs-lookup"><span data-stu-id="93ea8-115">User notebooks</span></span>
<span data-ttu-id="93ea8-116">Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="93ea8-116">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="93ea8-117">`me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="93ea8-117">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="93ea8-118">`users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="93ea8-118">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="93ea8-119">Use a API de [usuários](users.md).</span><span class="sxs-lookup"><span data-stu-id="93ea8-119">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="93ea8-120">**Observação:** Para obter as IDs de usuário, faça uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="93ea8-120">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="93ea8-121">Blocos de anotações de grupo</span><span class="sxs-lookup"><span data-stu-id="93ea8-121">Group notebooks</span></span>
<span data-ttu-id="93ea8-122">Para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="93ea8-122">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="93ea8-123">Blocos de anotações do SharePoint</span><span class="sxs-lookup"><span data-stu-id="93ea8-123">SharePoint site notebooks</span></span>

<span data-ttu-id="93ea8-124">Para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="93ea8-124">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

