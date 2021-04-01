---
title: Criar permissão
description: Crie um novo objeto de permissão.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 39e85b9ba4ef3269f46a2727a5771cadf3601e2a
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51490925"
---
# <a name="create-permission"></a><span data-ttu-id="d54e9-103">Criar permissão</span><span class="sxs-lookup"><span data-stu-id="d54e9-103">Create permission</span></span>
<span data-ttu-id="d54e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d54e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d54e9-105">Crie um novo [objeto de](../resources/permission.md) permissão em um site.</span><span class="sxs-lookup"><span data-stu-id="d54e9-105">Create a new [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="d54e9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d54e9-106">Permissions</span></span>
<span data-ttu-id="d54e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d54e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d54e9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d54e9-109">Permission type</span></span>                        | <span data-ttu-id="d54e9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d54e9-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d54e9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d54e9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d54e9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d54e9-112">Not supported.</span></span>
|<span data-ttu-id="d54e9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d54e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d54e9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d54e9-114">Not supported.</span></span>
|<span data-ttu-id="d54e9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d54e9-115">Application</span></span>                            | <span data-ttu-id="d54e9-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d54e9-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d54e9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d54e9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{sitesId}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="d54e9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d54e9-118">Request headers</span></span>
|<span data-ttu-id="d54e9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d54e9-119">Name</span></span>|<span data-ttu-id="d54e9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d54e9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d54e9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d54e9-121">Authorization</span></span>|<span data-ttu-id="d54e9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d54e9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d54e9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d54e9-124">Content-Type</span></span>|<span data-ttu-id="d54e9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d54e9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d54e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d54e9-127">Request body</span></span>
<span data-ttu-id="d54e9-128">No corpo da solicitação, fornece uma representação JSON do [objeto permission.](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="d54e9-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d54e9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d54e9-129">Response</span></span>

<span data-ttu-id="d54e9-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [de](../resources/permission.md) permissão no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d54e9-130">If successful, this method returns a `201 Created` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d54e9-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d54e9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d54e9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d54e9-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d54e9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d54e9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_permission_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{sitesId}/permissions
Content-Type: application/json

{
   "roles":[
      "write"
   ],
   "grantedToIdentities":[
      {
         "application":{
            "id":"89ea5c94-7736-4e25-95ad-3fa95f62b66e",
            "displayName":"Contoso Time Manager App"
         }
      }
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="d54e9-134">C#</span><span class="sxs-lookup"><span data-stu-id="d54e9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-permission-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d54e9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d54e9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-permission-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d54e9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d54e9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-permission-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d54e9-137">Java</span><span class="sxs-lookup"><span data-stu-id="d54e9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-permission-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d54e9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d54e9-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "id":"1",
   "roles":[
      "write"
   ],
   "grantedToIdentities":[
      {
         "application":{
            "id":"89ea5c94-7736-4e25-95ad-3fa95f62b66e",
            "displayName":"Contoso Time Manager App"
         }
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Create site permissions"
} -->
