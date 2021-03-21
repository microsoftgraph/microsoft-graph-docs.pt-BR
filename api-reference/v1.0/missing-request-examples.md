---
title: Definir /me como singleton
description: Essas são as coisas que eu tinha que adicionar nos documentos para garantir que o Markdown-Scanner
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 741a486bbaae5a666cb5c7d83f2a9c954523c2ec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955984"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="51305-103">Auxiliares (exemplos que não estão incluídos nos documentos)</span><span class="sxs-lookup"><span data-stu-id="51305-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="51305-104">Estas são as coisas que tive que adicionar aos documentos para garantir que a ferramenta Markdown-Scanner conseguiria lidar adequadamente com os documentos do Graph.</span><span class="sxs-lookup"><span data-stu-id="51305-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="51305-105">Definir /me como singleton</span><span class="sxs-lookup"><span data-stu-id="51305-105">Define the /me as singleton</span></span>


# <a name="http"></a>[<span data-ttu-id="51305-106">HTTP</span><span class="sxs-lookup"><span data-stu-id="51305-106">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_current_user" } -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me
```
# <a name="c"></a>[<span data-ttu-id="51305-107">C#</span><span class="sxs-lookup"><span data-stu-id="51305-107">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-current-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51305-108">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51305-108">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-current-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51305-109">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51305-109">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-current-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51305-110">Java</span><span class="sxs-lookup"><span data-stu-id="51305-110">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-current-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="51305-111">Defina as unidades como um conjunto de entidades consultável</span><span class="sxs-lookup"><span data-stu-id="51305-111">Define drives as an queryable entityset</span></span>

# <a name="http"></a>[<span data-ttu-id="51305-112">HTTP</span><span class="sxs-lookup"><span data-stu-id="51305-112">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```
# <a name="c"></a>[<span data-ttu-id="51305-113">C#</span><span class="sxs-lookup"><span data-stu-id="51305-113">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-from-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51305-114">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51305-114">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-from-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51305-115">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51305-115">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-from-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51305-116">Java</span><span class="sxs-lookup"><span data-stu-id="51305-116">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-from-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="51305-117">Defina os usuários como um conjunto de entidades consultável</span><span class="sxs-lookup"><span data-stu-id="51305-117">define users as an queryable entityset</span></span>


# <a name="http"></a>[<span data-ttu-id="51305-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="51305-118">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_users_1" } -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="51305-119">C#</span><span class="sxs-lookup"><span data-stu-id="51305-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51305-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51305-120">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51305-121">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51305-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51305-122">Java</span><span class="sxs-lookup"><span data-stu-id="51305-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d73
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Missing Requests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
