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
# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="1794b-104">Usar a API REST do OneNote</span><span class="sxs-lookup"><span data-stu-id="1794b-104">Use the OneNote REST API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1794b-105">O Microsoft Graph permite que o aplicativo obtenha acesso autorizado aos blocos de anotações, seções e páginas do OneNote de um usuário em uma conta pessoal ou de organização.</span><span class="sxs-lookup"><span data-stu-id="1794b-105">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="1794b-106">Com as [permissões delegadas ou de aplicativo apropriadas](/graph/permissions-reference#notes-permissions), seu aplicativo pode acessar os dados do OneNote do usuário conectado ou de qualquer usuário em um locatário.</span><span class="sxs-lookup"><span data-stu-id="1794b-106">With the [appropriate delegated or application permissions](/graph/permissions-reference#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span> 

## <a name="root-url"></a><span data-ttu-id="1794b-107">URL Raiz</span><span class="sxs-lookup"><span data-stu-id="1794b-107">Root URL</span></span>
<span data-ttu-id="1794b-108">A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para a API do OneNote.</span><span class="sxs-lookup"><span data-stu-id="1794b-108">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="1794b-109">O `version` segmento na URL representa a versão do Microsoft Graph que você deseja usar:</span><span class="sxs-lookup"><span data-stu-id="1794b-109">The `version` segment in the URL represents the version of Microsoft Graph that you want to use:</span></span>

- <span data-ttu-id="1794b-110">`v1.0` serve para o código de produção estável.</span><span class="sxs-lookup"><span data-stu-id="1794b-110">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="1794b-111">`beta` serve para experimentar um recurso que está em desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="1794b-111">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="1794b-112">Recursos e funcionalidades no ponto de extremidade beta podem mudar; Não recomendamos que você o use em seu código de produção.</span><span class="sxs-lookup"><span data-stu-id="1794b-112">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="1794b-113">O local pode ser blocos de anotações do usuário no Office 365 ou no OneDrive do consumidor, nos blocos de anotações de grupo ou em blocos de anotações de equipe hospedados no site do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="1794b-113">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![Pilha de desenvolvimento da API do OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="1794b-115">Blocos de anotações do usuário</span><span class="sxs-lookup"><span data-stu-id="1794b-115">User notebooks</span></span>
<span data-ttu-id="1794b-116">Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="1794b-116">To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="1794b-117">`me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado).</span><span class="sxs-lookup"><span data-stu-id="1794b-117">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="1794b-118">`users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="1794b-118">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="1794b-119">Use a API de [usuários](users.md) .</span><span class="sxs-lookup"><span data-stu-id="1794b-119">Use the [users](users.md) API.</span></span>
> <span data-ttu-id="1794b-120">**Observação:** Você pode obter IDs de usuário fazendo uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="1794b-120">**Note:** You can get user IDs by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="1794b-121">Blocos de anotações de grupo</span><span class="sxs-lookup"><span data-stu-id="1794b-121">Group notebooks</span></span>

<span data-ttu-id="1794b-122">Para acessar blocos de anotações pertencentes a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="1794b-122">To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="1794b-123">Blocos de anotações do site do SharePoint</span><span class="sxs-lookup"><span data-stu-id="1794b-123">SharePoint site notebooks</span></span>
<span data-ttu-id="1794b-124">Para acessar blocos de anotações pertencentes a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="1794b-124">To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

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
