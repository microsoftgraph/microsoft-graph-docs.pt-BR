---
author: chackman
ms.author: chackman
title: Listar itens seguidos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1efa34191693a0511e28d00ea29accd54877a586
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861576"
---
# <a name="list-followed-items"></a><span data-ttu-id="b5d41-102">Listar itens seguidos</span><span class="sxs-lookup"><span data-stu-id="b5d41-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5d41-103">Listar os [itens](../resources/driveitem.md) que foram seguidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b5d41-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="b5d41-104">Esta coleção inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades.</span><span class="sxs-lookup"><span data-stu-id="b5d41-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5d41-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5d41-105">Permissions</span></span>

<span data-ttu-id="b5d41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5d41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5d41-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5d41-108">Permission type</span></span>      | <span data-ttu-id="b5d41-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5d41-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5d41-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5d41-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5d41-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d41-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5d41-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5d41-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5d41-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5d41-113">Not supported.</span></span>    |
|<span data-ttu-id="b5d41-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5d41-114">Application</span></span> | <span data-ttu-id="b5d41-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d41-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5d41-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5d41-116">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5d41-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5d41-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5d41-118">C#</span><span class="sxs-lookup"><span data-stu-id="b5d41-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-followed-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5d41-119">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5d41-119">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-followed-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5d41-120">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b5d41-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-followed-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b5d41-121">Java</span><span class="sxs-lookup"><span data-stu-id="b5d41-121">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-followed-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="b5d41-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5d41-122">Response</span></span>

<span data-ttu-id="b5d41-123">Este método retorna uma coleção de recursos [driveItem](../resources/driveitem.md) para itens que o proprietário da unidade está seguindo.</span><span class="sxs-lookup"><span data-stu-id="b5d41-123">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="b5d41-124">Se não forem encontrados itens, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="b5d41-124">If no items were found, an empty collection is returned.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
  ]
}
-->
