---
title: Excluir cloudPcDeviceImage
description: Excluir um objeto cloudPcDeviceImage.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a65350162f7810da9c5d20b5f1982d75bc74ef4f
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563328"
---
# <a name="delete-cloudpcdeviceimage"></a><span data-ttu-id="4ea14-103">Excluir cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="4ea14-103">Delete cloudPcDeviceImage</span></span>

<span data-ttu-id="4ea14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea14-105">Excluir um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="4ea14-105">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="4ea14-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4ea14-106">Permissions</span></span>

<span data-ttu-id="4ea14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea14-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ea14-109">Permission type</span></span>|<span data-ttu-id="4ea14-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ea14-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ea14-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ea14-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ea14-112">CloudPC. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4ea14-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="4ea14-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ea14-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ea14-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ea14-114">Not supported.</span></span>|
|<span data-ttu-id="4ea14-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ea14-115">Application</span></span>|<span data-ttu-id="4ea14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ea14-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ea14-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea14-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4ea14-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea14-118">Request headers</span></span>

|<span data-ttu-id="4ea14-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4ea14-119">Name</span></span>|<span data-ttu-id="4ea14-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ea14-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ea14-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ea14-121">Authorization</span></span>|<span data-ttu-id="4ea14-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ea14-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ea14-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea14-124">Request body</span></span>

<span data-ttu-id="4ea14-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ea14-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ea14-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea14-126">Response</span></span>

<span data-ttu-id="4ea14-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4ea14-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4ea14-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4ea14-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ea14-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea14-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4ea14-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea14-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_deviceimages_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```
# <a name="c"></a>[<span data-ttu-id="4ea14-131">C#</span><span class="sxs-lookup"><span data-stu-id="4ea14-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-deviceimages-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ea14-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ea14-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-deviceimages-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ea14-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ea14-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-deviceimages-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ea14-134">Java</span><span class="sxs-lookup"><span data-stu-id="4ea14-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-deviceimages-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4ea14-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea14-135">Response</span></span>

<span data-ttu-id="4ea14-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4ea14-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
