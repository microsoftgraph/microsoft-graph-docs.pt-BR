---
title: Excluir updatableAsset
description: Exclua um objeto updatableAsset.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 7e266a24fd23858f60326e14b956cdf5ef731315
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240718"
---
# <a name="delete-updatableasset"></a><span data-ttu-id="20ddd-103">Excluir updatableAsset</span><span class="sxs-lookup"><span data-stu-id="20ddd-103">Delete updatableAsset</span></span>
<span data-ttu-id="20ddd-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="20ddd-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20ddd-105">[Exclua um objeto updatableAsset.](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="20ddd-105">Delete an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20ddd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20ddd-106">Permissions</span></span>
<span data-ttu-id="20ddd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20ddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20ddd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20ddd-109">Permission type</span></span>|<span data-ttu-id="20ddd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20ddd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20ddd-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20ddd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="20ddd-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20ddd-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="20ddd-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20ddd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20ddd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20ddd-114">Not supported.</span></span>|
|<span data-ttu-id="20ddd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20ddd-115">Application</span></span>|<span data-ttu-id="20ddd-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20ddd-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20ddd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20ddd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{updatableAssetId}
```

## <a name="request-headers"></a><span data-ttu-id="20ddd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20ddd-118">Request headers</span></span>
|<span data-ttu-id="20ddd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="20ddd-119">Name</span></span>|<span data-ttu-id="20ddd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="20ddd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20ddd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="20ddd-121">Authorization</span></span>|<span data-ttu-id="20ddd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20ddd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20ddd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20ddd-124">Request body</span></span>
<span data-ttu-id="20ddd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20ddd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20ddd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="20ddd-126">Response</span></span>

<span data-ttu-id="20ddd-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20ddd-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20ddd-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20ddd-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20ddd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20ddd-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="20ddd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="20ddd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_updatableasset"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetId}
```
# <a name="c"></a>[<span data-ttu-id="20ddd-132">C#</span><span class="sxs-lookup"><span data-stu-id="20ddd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20ddd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20ddd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20ddd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20ddd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20ddd-135">Java</span><span class="sxs-lookup"><span data-stu-id="20ddd-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20ddd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="20ddd-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

