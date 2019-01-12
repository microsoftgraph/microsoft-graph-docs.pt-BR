---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Listar os subsites de um site do SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f192826788df26b30701219527f5c7a6cd72049d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977133"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="45594-102">Enumerar subsites</span><span class="sxs-lookup"><span data-stu-id="45594-102">Enumerate subsites</span></span>

<span data-ttu-id="45594-103">Obtém uma coleção de subsites definidos para um [site][].</span><span class="sxs-lookup"><span data-stu-id="45594-103">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="45594-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="45594-105">Permissions</span></span>

<span data-ttu-id="45594-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45594-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45594-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45594-108">Permission type</span></span>      | <span data-ttu-id="45594-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45594-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45594-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45594-110">Delegated (work or school account)</span></span> | <span data-ttu-id="45594-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45594-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="45594-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45594-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45594-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45594-113">Not supported.</span></span>    |
|<span data-ttu-id="45594-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45594-114">Application</span></span> | <span data-ttu-id="45594-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45594-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45594-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45594-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="45594-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="45594-117">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites"
} -->
