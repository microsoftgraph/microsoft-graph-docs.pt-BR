---
title: Obter linkedResource
description: Leia as propriedades e os relacionamentos de um objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 830a7aba64221e1eb6918c0c66deb636a391d0d0
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873812"
---
# <a name="get-linkedresource"></a><span data-ttu-id="16b28-103">Obter linkedResource</span><span class="sxs-lookup"><span data-stu-id="16b28-103">Get linkedResource</span></span>
<span data-ttu-id="16b28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16b28-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16b28-105">Leia as propriedades e os relacionamentos de um [objeto linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="16b28-105">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="16b28-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="16b28-106">Permissions</span></span>
<span data-ttu-id="16b28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16b28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16b28-109">Permission type</span></span>|<span data-ttu-id="16b28-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16b28-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16b28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16b28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16b28-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16b28-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="16b28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16b28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16b28-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16b28-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="16b28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16b28-115">Application</span></span>|<span data-ttu-id="16b28-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="16b28-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="16b28-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16b28-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="16b28-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16b28-118">Request headers</span></span>
|<span data-ttu-id="16b28-119">Nome</span><span class="sxs-lookup"><span data-stu-id="16b28-119">Name</span></span>|<span data-ttu-id="16b28-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="16b28-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16b28-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="16b28-121">Authorization</span></span>|<span data-ttu-id="16b28-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16b28-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16b28-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16b28-124">Request body</span></span>
<span data-ttu-id="16b28-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16b28-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16b28-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b28-126">Response</span></span>

<span data-ttu-id="16b28-127">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16b28-127">If successful, this method returns a `200 OK` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16b28-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16b28-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16b28-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16b28-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="16b28-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="16b28-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```
# <a name="c"></a>[<span data-ttu-id="16b28-131">C#</span><span class="sxs-lookup"><span data-stu-id="16b28-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16b28-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16b28-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16b28-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16b28-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16b28-134">Java</span><span class="sxs-lookup"><span data-stu-id="16b28-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="16b28-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b28-135">Response</span></span>
<span data-ttu-id="16b28-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="16b28-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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


