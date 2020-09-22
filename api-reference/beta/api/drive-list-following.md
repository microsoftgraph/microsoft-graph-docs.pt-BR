---
author: chackman
description: Listar os itens que foram seguidos pelo usuário conectado.
title: Listar itens seguidos
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8fcba872a289b7985a013a0cbca06a0740977dbf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982224"
---
# <a name="list-followed-items"></a><span data-ttu-id="a877a-103">Listar itens seguidos</span><span class="sxs-lookup"><span data-stu-id="a877a-103">List followed items</span></span>

<span data-ttu-id="a877a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a877a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a877a-105">Listar os [itens](../resources/driveitem.md) que foram seguidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a877a-105">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="a877a-106">Esta coleção inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades.</span><span class="sxs-lookup"><span data-stu-id="a877a-106">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="a877a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a877a-107">Permissions</span></span>

<span data-ttu-id="a877a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a877a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a877a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a877a-110">Permission type</span></span>      | <span data-ttu-id="a877a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a877a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a877a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a877a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a877a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a877a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a877a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a877a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a877a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a877a-115">Not supported.</span></span>    |
|<span data-ttu-id="a877a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a877a-116">Application</span></span> | <span data-ttu-id="a877a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a877a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a877a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a877a-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="a877a-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="a877a-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/following
```
# <a name="c"></a>[<span data-ttu-id="a877a-120">C#</span><span class="sxs-lookup"><span data-stu-id="a877a-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-followed-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a877a-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a877a-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-followed-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a877a-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a877a-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-followed-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a877a-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="a877a-123">Response</span></span>

<span data-ttu-id="a877a-124">Este método retorna uma coleção de recursos [driveItem](../resources/driveitem.md) para itens que o proprietário da unidade está seguindo.</span><span class="sxs-lookup"><span data-stu-id="a877a-124">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="a877a-125">Se não forem encontrados itens, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="a877a-125">If no items were found, an empty collection is returned.</span></span>

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


