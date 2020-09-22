---
title: Obter linkedResource
description: Leia as propriedades e os relacionamentos de um objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d2c0ef4b2a10877aee0c9e956a43652bb42dc0ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999206"
---
# <a name="get-linkedresource"></a><span data-ttu-id="cc20e-103">Obter linkedResource</span><span class="sxs-lookup"><span data-stu-id="cc20e-103">Get linkedResource</span></span>
<span data-ttu-id="cc20e-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="cc20e-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="cc20e-105">Leia as propriedades e os relacionamentos de um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="cc20e-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc20e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc20e-106">Permissions</span></span>
<span data-ttu-id="cc20e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc20e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc20e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc20e-109">Permission type</span></span>|<span data-ttu-id="cc20e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc20e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc20e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc20e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cc20e-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc20e-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="cc20e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc20e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc20e-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc20e-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="cc20e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc20e-115">Application</span></span>|<span data-ttu-id="cc20e-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cc20e-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc20e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc20e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="cc20e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc20e-118">Request headers</span></span>
|<span data-ttu-id="cc20e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cc20e-119">Name</span></span>|<span data-ttu-id="cc20e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc20e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cc20e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc20e-121">Authorization</span></span>|<span data-ttu-id="cc20e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc20e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc20e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc20e-124">Request body</span></span>
<span data-ttu-id="cc20e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc20e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc20e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc20e-126">Response</span></span>

<span data-ttu-id="cc20e-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc20e-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc20e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cc20e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc20e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc20e-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cc20e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc20e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="cc20e-131">C#</span><span class="sxs-lookup"><span data-stu-id="cc20e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc20e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc20e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc20e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc20e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cc20e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc20e-134">Response</span></span>
<span data-ttu-id="cc20e-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cc20e-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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


