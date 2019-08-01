---
title: Definir /me como singleton
description: Essas são as coisas que eu precisava adicionar nos documentos para garantir que o verificador de redução
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 82dac0d1b01b9e06c68c8d48fa54d9e728b3a293
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030146"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="a3b5e-103">Auxiliares (exemplos que não estão incluídos nos documentos)</span><span class="sxs-lookup"><span data-stu-id="a3b5e-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="a3b5e-104">Estas são as coisas que tive que adicionar aos documentos para garantir que a ferramenta Markdown-Scanner conseguiria lidar adequadamente com os documentos do Graph.</span><span class="sxs-lookup"><span data-stu-id="a3b5e-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="a3b5e-105">Definir /me como singleton</span><span class="sxs-lookup"><span data-stu-id="a3b5e-105">Define the /me as singleton</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a3b5e-106">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3b5e-106">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3b5e-107">C#</span><span class="sxs-lookup"><span data-stu-id="a3b5e-107">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-current-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3b5e-108">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3b5e-108">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-current-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3b5e-109">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3b5e-109">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-current-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3b5e-110">Java</span><span class="sxs-lookup"><span data-stu-id="a3b5e-110">Java</span></span>](#tab/java)
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


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="a3b5e-111">Defina as unidades como um conjunto de entidades consultável</span><span class="sxs-lookup"><span data-stu-id="a3b5e-111">Define drives as an queryable entityset</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a3b5e-112">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3b5e-112">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3b5e-113">C#</span><span class="sxs-lookup"><span data-stu-id="a3b5e-113">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-from-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3b5e-114">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3b5e-114">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-from-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3b5e-115">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3b5e-115">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-from-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3b5e-116">Java</span><span class="sxs-lookup"><span data-stu-id="a3b5e-116">Java</span></span>](#tab/java)
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


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="a3b5e-117">Defina os usuários como um conjunto de entidades consultável</span><span class="sxs-lookup"><span data-stu-id="a3b5e-117">define users as an queryable entityset</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a3b5e-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3b5e-118">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3b5e-119">C#</span><span class="sxs-lookup"><span data-stu-id="a3b5e-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3b5e-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3b5e-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3b5e-121">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3b5e-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a3b5e-122">Java</span><span class="sxs-lookup"><span data-stu-id="a3b5e-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-users-java-snippets.md)]
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
