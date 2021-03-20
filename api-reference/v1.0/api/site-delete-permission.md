---
title: Permissão de exclusão
description: Exclua um objeto permission em um site.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 53649ddaccb9094f222a0aff6e07b2e52144cbe8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952702"
---
# <a name="delete-permission"></a><span data-ttu-id="7a650-103">Permissão de exclusão</span><span class="sxs-lookup"><span data-stu-id="7a650-103">Delete permission</span></span>
<span data-ttu-id="7a650-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a650-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a650-105">[Exclua um objeto](../resources/permission.md) permission em um site.</span><span class="sxs-lookup"><span data-stu-id="7a650-105">Delete a [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a650-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a650-106">Permissions</span></span>
<span data-ttu-id="7a650-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a650-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a650-109">Permission type</span></span>                        | <span data-ttu-id="7a650-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a650-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="7a650-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a650-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a650-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a650-112">Not supported.</span></span>
|<span data-ttu-id="7a650-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a650-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a650-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a650-114">Not supported.</span></span>
|<span data-ttu-id="7a650-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a650-115">Application</span></span>                            | <span data-ttu-id="7a650-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7a650-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="7a650-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a650-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="7a650-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a650-118">Request headers</span></span>
|<span data-ttu-id="7a650-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7a650-119">Name</span></span>|<span data-ttu-id="7a650-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a650-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a650-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a650-121">Authorization</span></span>|<span data-ttu-id="7a650-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a650-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a650-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a650-124">Request body</span></span>
<span data-ttu-id="7a650-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a650-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a650-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a650-126">Response</span></span>

<span data-ttu-id="7a650-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a650-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a650-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a650-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a650-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a650-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a650-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a650-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_permission_2"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
```
# <a name="c"></a>[<span data-ttu-id="7a650-132">C#</span><span class="sxs-lookup"><span data-stu-id="7a650-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a650-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a650-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a650-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a650-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a650-135">Java</span><span class="sxs-lookup"><span data-stu-id="7a650-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permission-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7a650-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a650-136">Response</span></span>
<span data-ttu-id="7a650-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a650-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Delete site permission"
} -->
