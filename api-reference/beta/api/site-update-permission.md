---
title: Atualizar permissão
description: Atualize o objeto permission em um site.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 27f006e5a2059662903f710ac994e176e1d51a22
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582596"
---
# <a name="update-permission"></a><span data-ttu-id="ba44d-103">Atualizar permissão</span><span class="sxs-lookup"><span data-stu-id="ba44d-103">Update permission</span></span>
<span data-ttu-id="ba44d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba44d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba44d-105">Atualize [o objeto](../resources/permission.md) permission em um site.</span><span class="sxs-lookup"><span data-stu-id="ba44d-105">Update the [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba44d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba44d-106">Permissions</span></span>
<span data-ttu-id="ba44d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba44d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba44d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba44d-109">Permission type</span></span>                        | <span data-ttu-id="ba44d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba44d-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="ba44d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba44d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba44d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba44d-112">Not supported.</span></span>
|<span data-ttu-id="ba44d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba44d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba44d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba44d-114">Not supported.</span></span>
|<span data-ttu-id="ba44d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba44d-115">Application</span></span>                            | <span data-ttu-id="ba44d-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ba44d-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="ba44d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba44d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="ba44d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba44d-118">Request headers</span></span>
|<span data-ttu-id="ba44d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ba44d-119">Name</span></span>|<span data-ttu-id="ba44d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba44d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ba44d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba44d-121">Authorization</span></span>|<span data-ttu-id="ba44d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba44d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ba44d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba44d-124">Content-Type</span></span>|<span data-ttu-id="ba44d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba44d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba44d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba44d-127">Request body</span></span>
<span data-ttu-id="ba44d-128">No corpo da solicitação, fornece uma representação JSON do [objeto permission.](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="ba44d-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ba44d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba44d-129">Response</span></span>

<span data-ttu-id="ba44d-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [de](../resources/permission.md) permissão no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba44d-130">If successful, this method returns a `200 OK` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba44d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba44d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba44d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba44d-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ba44d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba44d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permission_from_"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/sites/{sitesId}/permissions/{permissionId}
Content-Type: application/json

{
  "roles": ["read"]
}
```
# <a name="c"></a>[<span data-ttu-id="ba44d-134">C#</span><span class="sxs-lookup"><span data-stu-id="ba44d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba44d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba44d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba44d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba44d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba44d-137">Java</span><span class="sxs-lookup"><span data-stu-id="ba44d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ba44d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba44d-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"2",
   "roles":[
      "read"
   ],
   "grantedToIdentities":[
      {
         "application":{
            "id":"89ea5c94-7736-4e25-95ad-3fa95f62b66e",
            "displayName":"Fabrikam Dashboard App"
         }
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Update site permission"
} -->
