---
title: Excluir implantação
description: Excluir um objeto de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 3baf7f9d163c7f1f4beb8967ca8cb94b53fb95f5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241370"
---
# <a name="delete-deployment"></a><span data-ttu-id="2441b-103">Excluir implantação</span><span class="sxs-lookup"><span data-stu-id="2441b-103">Delete deployment</span></span>
<span data-ttu-id="2441b-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="2441b-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2441b-105">Excluir um [objeto de](../resources/windowsupdates-deployment.md) implantação.</span><span class="sxs-lookup"><span data-stu-id="2441b-105">Delete a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2441b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2441b-106">Permissions</span></span>
<span data-ttu-id="2441b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2441b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2441b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2441b-109">Permission type</span></span>|<span data-ttu-id="2441b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2441b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2441b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2441b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2441b-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2441b-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="2441b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2441b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2441b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2441b-114">Not supported.</span></span>|
|<span data-ttu-id="2441b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2441b-115">Application</span></span>|<span data-ttu-id="2441b-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2441b-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2441b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2441b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a><span data-ttu-id="2441b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2441b-118">Request headers</span></span>
|<span data-ttu-id="2441b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2441b-119">Name</span></span>|<span data-ttu-id="2441b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2441b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2441b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2441b-121">Authorization</span></span>|<span data-ttu-id="2441b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2441b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2441b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2441b-124">Request body</span></span>
<span data-ttu-id="2441b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2441b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2441b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2441b-126">Response</span></span>

<span data-ttu-id="2441b-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2441b-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2441b-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2441b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2441b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2441b-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2441b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2441b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_deployment"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}
```
# <a name="c"></a>[<span data-ttu-id="2441b-132">C#</span><span class="sxs-lookup"><span data-stu-id="2441b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2441b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2441b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2441b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2441b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2441b-135">Java</span><span class="sxs-lookup"><span data-stu-id="2441b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2441b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2441b-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

