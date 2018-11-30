---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Listar os subsites de um site do SharePoint
ms.openlocfilehash: 2f35e891afc3cbeaf0504c3dd8008bafb23ecd52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036312"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="f9cbd-102">Enumerar subsites</span><span class="sxs-lookup"><span data-stu-id="f9cbd-102">Enumerate subsites</span></span>

> <span data-ttu-id="f9cbd-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9cbd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9cbd-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9cbd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9cbd-105">Obtém uma coleção de subsites definidos para um [site][].</span><span class="sxs-lookup"><span data-stu-id="f9cbd-105">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="f9cbd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9cbd-107">Permissions</span></span>

<span data-ttu-id="f9cbd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9cbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9cbd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9cbd-110">Permission type</span></span>      | <span data-ttu-id="f9cbd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9cbd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9cbd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9cbd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f9cbd-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9cbd-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f9cbd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9cbd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9cbd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9cbd-115">Not supported.</span></span>    |
|<span data-ttu-id="f9cbd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9cbd-116">Application</span></span> | <span data-ttu-id="f9cbd-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9cbd-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9cbd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9cbd-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="f9cbd-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9cbd-119">Response</span></span>

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
