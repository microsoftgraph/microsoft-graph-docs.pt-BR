---
title: 'cloudPcDeviceImage: reupload'
description: Recarregue um objeto cloudPcDeviceImage.
author: RuiHou105
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: ab636894279317ef18b4f41eb86081ac159ded59
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367042"
---
# <a name="cloudpcdeviceimage-reupload"></a><span data-ttu-id="9ab4b-103">cloudPcDeviceImage: reupload</span><span class="sxs-lookup"><span data-stu-id="9ab4b-103">cloudPcDeviceImage: reupload</span></span>

<span data-ttu-id="9ab4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ab4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ab4b-105">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span><span class="sxs-lookup"><span data-stu-id="9ab4b-105">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="9ab4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ab4b-106">Permissions</span></span>

<span data-ttu-id="9ab4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ab4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ab4b-109">Permission type</span></span>|<span data-ttu-id="9ab4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ab4b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ab4b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ab4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ab4b-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ab4b-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="9ab4b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ab4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ab4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ab4b-114">Not supported.</span></span>|
|<span data-ttu-id="9ab4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ab4b-115">Application</span></span>|<span data-ttu-id="9ab4b-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ab4b-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ab4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab4b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```

## <a name="request-headers"></a><span data-ttu-id="9ab4b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab4b-118">Request headers</span></span>

|<span data-ttu-id="9ab4b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9ab4b-119">Name</span></span>|<span data-ttu-id="9ab4b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab4b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9ab4b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ab4b-121">Authorization</span></span>|<span data-ttu-id="9ab4b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ab4b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ab4b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab4b-124">Request body</span></span>

<span data-ttu-id="9ab4b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ab4b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ab4b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab4b-126">Response</span></span>

<span data-ttu-id="9ab4b-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9ab4b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9ab4b-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9ab4b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ab4b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab4b-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "reupload_deviceimages_from_virtualendpoint"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```

### <a name="response"></a><span data-ttu-id="9ab4b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab4b-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
