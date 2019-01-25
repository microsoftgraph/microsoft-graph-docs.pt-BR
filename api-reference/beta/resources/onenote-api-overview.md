---
title: Usar a API REST do OneNote
description: 'O Microsoft Graph permite que o seu aplicativo obter acesso autorizado a um usuário OneNote blocos de anotações, seções e páginas em uma conta pessoal ou organização. Com o apropriado delegada ou permissões de aplicativo, seu aplicativo podem acessar os dados de OneNote do usuário conectado ou a qualquer usuário em um locatário. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7db3024224dde7ee4c95d2e3840187709471cecd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525623"
---
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="84503-104">Usar a API REST do OneNote</span><span class="sxs-lookup"><span data-stu-id="84503-104">Use the OneNote REST API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84503-105">O Microsoft Graph permite que o seu aplicativo obter acesso autorizado a um usuário OneNote blocos de anotações, seções e páginas em uma conta pessoal ou organização.</span><span class="sxs-lookup"><span data-stu-id="84503-105">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="84503-106">Com as [permissões apropriadas de delegada ou de aplicativos](/graph/permissions-reference#notes-permissions), seu aplicativo pode acessar os dados de OneNote do usuário conectado ou a qualquer usuário em um locatário.</span><span class="sxs-lookup"><span data-stu-id="84503-106">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="84503-107">URL raiz</span><span class="sxs-lookup"><span data-stu-id="84503-107">Root URL</span></span>
<span data-ttu-id="84503-108">A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para o OneNote.</span><span class="sxs-lookup"><span data-stu-id="84503-108">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="84503-109">O `version` segmento na URL representa a versão do Microsoft Graph que você deseja usar:</span><span class="sxs-lookup"><span data-stu-id="84503-109">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="84503-110">`v1.0` serve para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="84503-110">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="84503-111">`beta` serve para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="84503-111">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="84503-112">Recursos e funcionalidades no ponto de extremidade beta podem ser alterado; não recomendamos que você usá-lo em seu código de produção.</span><span class="sxs-lookup"><span data-stu-id="84503-112">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="84503-113">A localização pode ser blocos de anotações do usuário no Office 365 ou OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações hospedado no site de equipe do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="84503-113">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![Pilha do desenvolvimento de API do OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="84503-115">Blocos de anotações do usuário</span><span class="sxs-lookup"><span data-stu-id="84503-115">User notebooks</span></span>
<span data-ttu-id="84503-116">Para acessar os blocos de anotações pessoais consumidor OneDrive ou OneDrive for Business, use um dos seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="84503-116">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="84503-117">`me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="84503-117">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="84503-118">`users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="84503-118">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="84503-119">Use os [usuários](users.md) API.</span><span class="sxs-lookup"><span data-stu-id="84503-119">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="84503-120">**Observação:** para obter as ids de usuário, faça uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="84503-120">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="84503-121">Blocos de anotações do grupo</span><span class="sxs-lookup"><span data-stu-id="84503-121">Group notebooks</span></span>

<span data-ttu-id="84503-122">Para acessar os blocos de anotações pertencentes a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="84503-122">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="84503-123">Blocos de anotações do site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="84503-123">SharePoint site notebooks</span></span>
<span data-ttu-id="84503-124">Para acessar os blocos de anotações pertencentes a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="84503-124">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

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
