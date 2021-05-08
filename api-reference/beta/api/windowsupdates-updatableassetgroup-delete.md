---
title: Excluir updatableAssetGroup
description: Exclua um objeto updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 1410314bfe4f3de461deb0a1da9f76330833096c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239318"
---
# <a name="delete-updatableassetgroup"></a><span data-ttu-id="fd3a9-103">Excluir updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="fd3a9-103">Delete updatableAssetGroup</span></span>
<span data-ttu-id="fd3a9-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="fd3a9-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd3a9-105">[Exclua um objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="fd3a9-105">Delete an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="fd3a9-106">Quando um [objeto updatableAssetGroup,](../resources/windowsupdates-updatableassetgroup.md) seus objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) do membro não são excluídos.</span><span class="sxs-lookup"><span data-stu-id="fd3a9-106">When an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object, its member [updatableAsset](../resources/windowsupdates-updatableasset.md) objects are not deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd3a9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd3a9-107">Permissions</span></span>
<span data-ttu-id="fd3a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd3a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd3a9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd3a9-110">Permission type</span></span>|<span data-ttu-id="fd3a9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd3a9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd3a9-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd3a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd3a9-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd3a9-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="fd3a9-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd3a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd3a9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd3a9-115">Not supported.</span></span>|
|<span data-ttu-id="fd3a9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd3a9-116">Application</span></span>|<span data-ttu-id="fd3a9-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd3a9-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd3a9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd3a9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="fd3a9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd3a9-119">Request headers</span></span>
|<span data-ttu-id="fd3a9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fd3a9-120">Name</span></span>|<span data-ttu-id="fd3a9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd3a9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fd3a9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd3a9-122">Authorization</span></span>|<span data-ttu-id="fd3a9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd3a9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd3a9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd3a9-125">Request body</span></span>
<span data-ttu-id="fd3a9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd3a9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd3a9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd3a9-127">Response</span></span>

<span data-ttu-id="fd3a9-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd3a9-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd3a9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fd3a9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fd3a9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd3a9-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fd3a9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd3a9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_updatableassetgroup"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```
# <a name="c"></a>[<span data-ttu-id="fd3a9-133">C#</span><span class="sxs-lookup"><span data-stu-id="fd3a9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-updatableassetgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd3a9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd3a9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-updatableassetgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd3a9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd3a9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-updatableassetgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd3a9-136">Java</span><span class="sxs-lookup"><span data-stu-id="fd3a9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-updatableassetgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fd3a9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd3a9-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

