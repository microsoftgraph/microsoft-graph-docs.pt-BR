---
title: 'cloudPcDeviceImage: reupload'
description: Recarregue um objeto cloudPcDeviceImage.
author: RuiHou105
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 8e359f749f0b932f3061bf8750fcf7992fe23302
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439473"
---
# <a name="cloudpcdeviceimage-reupload"></a><span data-ttu-id="b9348-103">cloudPcDeviceImage: reupload</span><span class="sxs-lookup"><span data-stu-id="b9348-103">cloudPcDeviceImage: reupload</span></span>

<span data-ttu-id="b9348-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9348-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9348-105">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span><span class="sxs-lookup"><span data-stu-id="b9348-105">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="b9348-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b9348-106">Permissions</span></span>

<span data-ttu-id="b9348-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9348-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9348-109">Permission type</span></span>|<span data-ttu-id="b9348-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9348-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9348-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9348-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9348-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9348-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="b9348-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9348-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9348-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9348-114">Not supported.</span></span>|
|<span data-ttu-id="b9348-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9348-115">Application</span></span>|<span data-ttu-id="b9348-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9348-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9348-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9348-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```

## <a name="request-headers"></a><span data-ttu-id="b9348-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9348-118">Request headers</span></span>

|<span data-ttu-id="b9348-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b9348-119">Name</span></span>|<span data-ttu-id="b9348-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9348-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9348-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9348-121">Authorization</span></span>|<span data-ttu-id="b9348-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9348-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9348-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9348-124">Request body</span></span>

<span data-ttu-id="b9348-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9348-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9348-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9348-126">Response</span></span>

<span data-ttu-id="b9348-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b9348-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b9348-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b9348-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9348-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9348-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b9348-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9348-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reupload_deviceimages_from_virtualendpoint"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```
# <a name="c"></a>[<span data-ttu-id="b9348-131">C#</span><span class="sxs-lookup"><span data-stu-id="b9348-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reupload-deviceimages-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9348-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9348-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reupload-deviceimages-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9348-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9348-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reupload-deviceimages-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9348-134">Java</span><span class="sxs-lookup"><span data-stu-id="b9348-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reupload-deviceimages-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9348-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9348-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
