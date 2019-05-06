---
author: chackman
ms.author: chackman
title: Listar itens seguidos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1892b6c9adac3c41cf99bf755aa8d67d51a0066e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589740"
---
# <a name="list-followed-items"></a><span data-ttu-id="8cf56-102">Listar itens seguidos</span><span class="sxs-lookup"><span data-stu-id="8cf56-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cf56-103">Listar os [itens](../resources/driveitem.md) que foram seguidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8cf56-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="8cf56-104">Esta coleção inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades.</span><span class="sxs-lookup"><span data-stu-id="8cf56-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cf56-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cf56-105">Permissions</span></span>

<span data-ttu-id="8cf56-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cf56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cf56-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cf56-108">Permission type</span></span>      | <span data-ttu-id="8cf56-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cf56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cf56-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cf56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8cf56-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cf56-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8cf56-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cf56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cf56-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cf56-113">Not supported.</span></span>    |
|<span data-ttu-id="8cf56-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cf56-114">Application</span></span> | <span data-ttu-id="8cf56-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cf56-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cf56-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cf56-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="8cf56-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cf56-117">Response</span></span>

<span data-ttu-id="8cf56-118">Este método retorna uma coleção de recursos [driveItem](../resources/driveitem.md) para itens que o proprietário da unidade está seguindo.</span><span class="sxs-lookup"><span data-stu-id="8cf56-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="8cf56-119">Se não forem encontrados itens, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="8cf56-119">If no items were found, an empty collection is returned.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8cf56-120">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8cf56-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8cf56-121">Basic</span><span class="sxs-lookup"><span data-stu-id="8cf56-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-followed-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8cf56-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cf56-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-followed-items-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
