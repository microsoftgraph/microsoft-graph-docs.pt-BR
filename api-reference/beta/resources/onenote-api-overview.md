---
title: Usar a API REST do OneNote
description: 'O Microsoft Graph permite que o seu aplicativo obter acesso autorizado a um usuário OneNote blocos de anotações, seções e páginas em uma conta pessoal ou organização. Com o apropriado delegada ou permissões de aplicativo, seu aplicativo podem acessar os dados de OneNote do usuário conectado ou a qualquer usuário em um locatário. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ff17f7fbe5f15752bc272b79f3f741180f8d6417
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952997"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="c3026-104">Usar a API REST do OneNote</span><span class="sxs-lookup"><span data-stu-id="c3026-104">Use the OneNote REST API</span></span>

> <span data-ttu-id="c3026-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c3026-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3026-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c3026-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3026-107">O Microsoft Graph permite que o seu aplicativo obter acesso autorizado a um usuário OneNote blocos de anotações, seções e páginas em uma conta pessoal ou organização.</span><span class="sxs-lookup"><span data-stu-id="c3026-107">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="c3026-108">Com as [permissões apropriadas de delegada ou de aplicativos](/graph/permissions-reference#notes-permissions), seu aplicativo pode acessar os dados de OneNote do usuário conectado ou a qualquer usuário em um locatário.</span><span class="sxs-lookup"><span data-stu-id="c3026-108">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="c3026-109">URL raiz</span><span class="sxs-lookup"><span data-stu-id="c3026-109">Root URL</span></span>
<span data-ttu-id="c3026-110">A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para o OneNote.</span><span class="sxs-lookup"><span data-stu-id="c3026-110">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="c3026-111">O `version` segmento na URL representa a versão do Microsoft Graph que você deseja usar:</span><span class="sxs-lookup"><span data-stu-id="c3026-111">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="c3026-112">`v1.0` serve para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="c3026-112">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="c3026-113">`beta` serve para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="c3026-113">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="c3026-114">Recursos e funcionalidades no ponto de extremidade beta podem ser alterado; não recomendamos que você usá-lo em seu código de produção.</span><span class="sxs-lookup"><span data-stu-id="c3026-114">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="c3026-115">O local pode ser blocos de anotações do usuário no Office 365 ou consumidor OneDrive, blocos de anotações do grupo ou blocos de anotações do SharePoint team site hospedado no Office 365.</span><span class="sxs-lookup"><span data-stu-id="c3026-115">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![Pilha do desenvolvimento de API do OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="c3026-117">Blocos de anotações do usuário</span><span class="sxs-lookup"><span data-stu-id="c3026-117">User notebooks</span></span>
<span data-ttu-id="c3026-118">Para acessar os blocos de anotações pessoais consumidor OneDrive ou OneDrive for Business, use um dos seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="c3026-118">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="c3026-119">`me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="c3026-119">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="c3026-120">`users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="c3026-120">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="c3026-121">Use os [usuários](users.md) API.</span><span class="sxs-lookup"><span data-stu-id="c3026-121">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="c3026-122">**Observação:** Você pode obter IDs de usuário fazendo uma solicitação GET na `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="c3026-122">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="c3026-123">Blocos de anotações do grupo</span><span class="sxs-lookup"><span data-stu-id="c3026-123">Group notebooks</span></span>

<span data-ttu-id="c3026-124">Para acessar os blocos de anotações pertencentes a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="c3026-124">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="c3026-125">Blocos de anotações do site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="c3026-125">SharePoint site notebooks</span></span>
<span data-ttu-id="c3026-126">Para acessar os blocos de anotações pertencentes a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="c3026-126">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
