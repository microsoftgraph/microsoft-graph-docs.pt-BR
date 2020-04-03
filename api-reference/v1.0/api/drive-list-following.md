---
author: learafa
description: Listar os itens que foram seguidos pelo usuário conectado.
title: Listar itens seguidos
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 10c3dba22df34b15f5c9cb17eefe7586ce4fb872
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124319"
---
# <a name="list-followed-items"></a><span data-ttu-id="3da93-103">Listar itens seguidos</span><span class="sxs-lookup"><span data-stu-id="3da93-103">List followed items</span></span>

<span data-ttu-id="3da93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3da93-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3da93-105">Listar os [itens](../resources/driveitem.md) que foram seguidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="3da93-105">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="3da93-106">Esta coleção inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades.</span><span class="sxs-lookup"><span data-stu-id="3da93-106">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="3da93-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3da93-107">Permissions</span></span>

<span data-ttu-id="3da93-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3da93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3da93-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3da93-110">Permission type</span></span>      | <span data-ttu-id="3da93-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3da93-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3da93-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3da93-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3da93-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da93-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3da93-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3da93-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3da93-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3da93-115">Not supported.</span></span>    |
|<span data-ttu-id="3da93-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3da93-116">Application</span></span> | <span data-ttu-id="3da93-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da93-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3da93-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3da93-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="3da93-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="3da93-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/following
```
# <a name="c"></a>[<span data-ttu-id="3da93-120">C#</span><span class="sxs-lookup"><span data-stu-id="3da93-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-followed-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3da93-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3da93-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-followed-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3da93-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3da93-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-followed-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3da93-123">Java</span><span class="sxs-lookup"><span data-stu-id="3da93-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-followed-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="3da93-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="3da93-124">Response</span></span>

<span data-ttu-id="3da93-125">Este método retorna uma coleção de recursos [driveItem](../resources/driveitem.md) para itens que o proprietário da unidade está seguindo.</span><span class="sxs-lookup"><span data-stu-id="3da93-125">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="3da93-126">Se não forem encontrados itens, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="3da93-126">If no items were found, an empty collection is returned.</span></span>

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
