---
title: Excluir cloudPcDeviceImage
description: Excluir um objeto cloudPcDeviceImage.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e6b5ad15ec2bf768a9b02cb49289c8028699f3ea
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378207"
---
# <a name="delete-cloudpcdeviceimage"></a><span data-ttu-id="b021e-103">Excluir cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="b021e-103">Delete cloudPcDeviceImage</span></span>

<span data-ttu-id="b021e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b021e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b021e-105">Excluir um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="b021e-105">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b021e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b021e-106">Permissions</span></span>

<span data-ttu-id="b021e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b021e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b021e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b021e-109">Permission type</span></span>|<span data-ttu-id="b021e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b021e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b021e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b021e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b021e-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b021e-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="b021e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b021e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b021e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b021e-114">Not supported.</span></span>|
|<span data-ttu-id="b021e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b021e-115">Application</span></span>|<span data-ttu-id="b021e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b021e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b021e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b021e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b021e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b021e-118">Request headers</span></span>

|<span data-ttu-id="b021e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b021e-119">Name</span></span>|<span data-ttu-id="b021e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b021e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b021e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b021e-121">Authorization</span></span>|<span data-ttu-id="b021e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b021e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b021e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b021e-124">Request body</span></span>

<span data-ttu-id="b021e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b021e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b021e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b021e-126">Response</span></span>

<span data-ttu-id="b021e-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b021e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b021e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b021e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b021e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b021e-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_deviceimages_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```

### <a name="response"></a><span data-ttu-id="b021e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b021e-130">Response</span></span>

<span data-ttu-id="b021e-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b021e-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
