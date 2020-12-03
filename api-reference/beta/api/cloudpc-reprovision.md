---
title: 'cloudPC: reprovisionar'
description: Reconfigurar um PC de nuvem específico.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 6fe8b4a4a588c3ce469f300b397c767f33eed221
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563342"
---
# <a name="cloudpc-reprovision"></a><span data-ttu-id="0d39f-103">cloudPC: reprovisionar</span><span class="sxs-lookup"><span data-stu-id="0d39f-103">cloudPC: reprovision</span></span>

<span data-ttu-id="0d39f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d39f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d39f-105">Reconfigurar um PC de nuvem específico.</span><span class="sxs-lookup"><span data-stu-id="0d39f-105">Reprovision a specific cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="0d39f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0d39f-106">Permissions</span></span>

<span data-ttu-id="0d39f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d39f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d39f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d39f-109">Permission type</span></span>|<span data-ttu-id="0d39f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0d39f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d39f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d39f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d39f-112">CloudPC. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0d39f-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="0d39f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d39f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d39f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d39f-114">Not supported.</span></span>|
|<span data-ttu-id="0d39f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d39f-115">Application</span></span>|<span data-ttu-id="0d39f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d39f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d39f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d39f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

## <a name="request-headers"></a><span data-ttu-id="0d39f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d39f-118">Request headers</span></span>

|<span data-ttu-id="0d39f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0d39f-119">Name</span></span>|<span data-ttu-id="0d39f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d39f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0d39f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d39f-121">Authorization</span></span>|<span data-ttu-id="0d39f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d39f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d39f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d39f-124">Request body</span></span>

<span data-ttu-id="0d39f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d39f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d39f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d39f-126">Response</span></span>

<span data-ttu-id="0d39f-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d39f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0d39f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d39f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d39f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d39f-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0d39f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d39f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```
# <a name="c"></a>[<span data-ttu-id="0d39f-131">C#</span><span class="sxs-lookup"><span data-stu-id="0d39f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d39f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d39f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d39f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d39f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d39f-134">Java</span><span class="sxs-lookup"><span data-stu-id="0d39f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0d39f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d39f-135">Response</span></span>

<span data-ttu-id="0d39f-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0d39f-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
