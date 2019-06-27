---
author: chackman
ms.author: chackman
title: Listar itens seguidos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0c7f7a072fb7960b1bc160c06367252fd183f9e4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260330"
---
# <a name="list-followed-items"></a><span data-ttu-id="7ed1f-102">Listar itens seguidos</span><span class="sxs-lookup"><span data-stu-id="7ed1f-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ed1f-103">Listar os [itens](../resources/driveitem.md) que foram seguidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="7ed1f-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="7ed1f-104">Esta coleção inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades.</span><span class="sxs-lookup"><span data-stu-id="7ed1f-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ed1f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ed1f-105">Permissions</span></span>

<span data-ttu-id="7ed1f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ed1f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ed1f-108">Permission type</span></span>      | <span data-ttu-id="7ed1f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ed1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ed1f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ed1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ed1f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed1f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ed1f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ed1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ed1f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed1f-113">Not supported.</span></span>    |
|<span data-ttu-id="7ed1f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ed1f-114">Application</span></span> | <span data-ttu-id="7ed1f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed1f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ed1f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ed1f-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="7ed1f-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed1f-117">Response</span></span>

<span data-ttu-id="7ed1f-118">Este método retorna uma coleção de recursos [driveItem](../resources/driveitem.md) para itens que o proprietário da unidade está seguindo.</span><span class="sxs-lookup"><span data-stu-id="7ed1f-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="7ed1f-119">Se não forem encontrados itens, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="7ed1f-119">If no items were found, an empty collection is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7ed1f-120">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="7ed1f-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7ed1f-121">C#</span><span class="sxs-lookup"><span data-stu-id="7ed1f-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-followed-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ed1f-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ed1f-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-followed-items-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ed1f-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7ed1f-123">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-followed-items-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
