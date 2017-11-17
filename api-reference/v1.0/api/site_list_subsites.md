---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Listar os subsites de um site do SharePoint
ms.openlocfilehash: a2acf82fca78249e6ea8d05a4a95f88ed741c913
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="enumerate-subsites"></a><span data-ttu-id="6ce2d-102">Enumerar subsites</span><span class="sxs-lookup"><span data-stu-id="6ce2d-102">Enumerate subsites</span></span>

<span data-ttu-id="6ce2d-103">Obtém uma coleção de subsites definidos para um [site][].</span><span class="sxs-lookup"><span data-stu-id="6ce2d-103">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="6ce2d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ce2d-105">Permissions</span></span>

<span data-ttu-id="6ce2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ce2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6ce2d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ce2d-108">Permission type</span></span>      | <span data-ttu-id="6ce2d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ce2d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ce2d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ce2d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ce2d-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce2d-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6ce2d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ce2d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ce2d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ce2d-113">Not supported.</span></span>    |
|<span data-ttu-id="6ce2d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ce2d-114">Application</span></span> | <span data-ttu-id="6ce2d-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce2d-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ce2d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ce2d-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="6ce2d-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ce2d-117">Response</span></span>

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
