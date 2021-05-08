---
title: Criar updatableAssetGroup
description: Crie um novo objeto updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 4a7bb68439cd3fd2eade0eaf11b43e2bbf51a5b2
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238435"
---
# <a name="create-updatableassetgroup"></a><span data-ttu-id="5a869-103">Criar updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="5a869-103">Create updatableAssetGroup</span></span>
<span data-ttu-id="5a869-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="5a869-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a869-105">Crie um novo [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5a869-105">Create a new [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="5a869-106">O **recurso updatableAssetGroup** herda de [updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="5a869-106">The **updatableAssetGroup** resource inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5a869-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a869-107">Permissions</span></span>
<span data-ttu-id="5a869-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a869-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a869-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a869-110">Permission type</span></span>|<span data-ttu-id="5a869-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a869-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a869-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a869-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a869-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a869-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="5a869-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a869-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a869-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a869-115">Not supported.</span></span>|
|<span data-ttu-id="5a869-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a869-116">Application</span></span>|<span data-ttu-id="5a869-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a869-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a869-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a869-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets
```

## <a name="request-headers"></a><span data-ttu-id="5a869-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a869-119">Request headers</span></span>
|<span data-ttu-id="5a869-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5a869-120">Name</span></span>|<span data-ttu-id="5a869-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a869-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5a869-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a869-122">Authorization</span></span>|<span data-ttu-id="5a869-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a869-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5a869-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a869-125">Content-Type</span></span>|<span data-ttu-id="5a869-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a869-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a869-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a869-128">Request body</span></span>
<span data-ttu-id="5a869-129">No corpo da solicitação, fornece uma representação JSON do [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5a869-129">In the request body, supply a JSON representation of the [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="5a869-130">Nenhuma propriedade é necessária.</span><span class="sxs-lookup"><span data-stu-id="5a869-130">No properties are required.</span></span>


## <a name="response"></a><span data-ttu-id="5a869-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a869-131">Response</span></span>

<span data-ttu-id="5a869-132">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a869-132">If successful, this method returns a `201 Created` response code and an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a869-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5a869-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a869-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a869-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5a869-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a869-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_updatableassetgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets
Content-Type: application/json
Content-length: 76

{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup"
}
```
# <a name="c"></a>[<span data-ttu-id="5a869-136">C#</span><span class="sxs-lookup"><span data-stu-id="5a869-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-updatableassetgroup-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a869-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a869-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-updatableassetgroup-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a869-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a869-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-updatableassetgroup-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a869-139">Java</span><span class="sxs-lookup"><span data-stu-id="5a869-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-updatableassetgroup-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5a869-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a869-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
}
```

