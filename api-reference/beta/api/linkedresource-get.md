---
title: Obter linkedResource
description: Leia as propriedades e as relações de um objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ef0d78c12812f16338c04455827a683319478f57
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961661"
---
# <a name="get-linkedresource"></a><span data-ttu-id="a2b9b-103">Obter linkedResource</span><span class="sxs-lookup"><span data-stu-id="a2b9b-103">Get linkedResource</span></span>
<span data-ttu-id="a2b9b-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="a2b9b-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="a2b9b-105">Leia as propriedades e as relações de um [objeto linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="a2b9b-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2b9b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2b9b-106">Permissions</span></span>
<span data-ttu-id="a2b9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2b9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2b9b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2b9b-109">Permission type</span></span>|<span data-ttu-id="a2b9b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2b9b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2b9b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2b9b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a2b9b-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2b9b-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a2b9b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2b9b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2b9b-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2b9b-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a2b9b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2b9b-115">Application</span></span>|<span data-ttu-id="a2b9b-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a2b9b-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2b9b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2b9b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="a2b9b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b9b-118">Request headers</span></span>
|<span data-ttu-id="a2b9b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a2b9b-119">Name</span></span>|<span data-ttu-id="a2b9b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2b9b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a2b9b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2b9b-121">Authorization</span></span>|<span data-ttu-id="a2b9b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2b9b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2b9b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b9b-124">Request body</span></span>
<span data-ttu-id="a2b9b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2b9b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2b9b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2b9b-126">Response</span></span>

<span data-ttu-id="a2b9b-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2b9b-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2b9b-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a2b9b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a2b9b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2b9b-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a2b9b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2b9b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="a2b9b-131">C#</span><span class="sxs-lookup"><span data-stu-id="a2b9b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2b9b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2b9b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2b9b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2b9b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2b9b-134">Java</span><span class="sxs-lookup"><span data-stu-id="a2b9b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a2b9b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2b9b-135">Response</span></span>
<span data-ttu-id="a2b9b-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a2b9b-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
     "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
  }
}
```


