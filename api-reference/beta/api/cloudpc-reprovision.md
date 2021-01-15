---
title: 'cloudPC: reprovisionamento'
description: Reprovisione um computador em nuvem específico.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7a887ced74a6b0eb53e1516f314cc2be5ff96428
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872874"
---
# <a name="cloudpc-reprovision"></a><span data-ttu-id="a8880-103">cloudPC: reprovisionamento</span><span class="sxs-lookup"><span data-stu-id="a8880-103">cloudPC: reprovision</span></span>

<span data-ttu-id="a8880-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8880-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8880-105">Reprovisione um computador em nuvem específico.</span><span class="sxs-lookup"><span data-stu-id="a8880-105">Reprovision a specific cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="a8880-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8880-106">Permissions</span></span>

<span data-ttu-id="a8880-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8880-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8880-109">Permission type</span></span>|<span data-ttu-id="a8880-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8880-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8880-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8880-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a8880-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8880-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a8880-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8880-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8880-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8880-114">Not supported.</span></span>|
|<span data-ttu-id="a8880-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8880-115">Application</span></span>|<span data-ttu-id="a8880-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8880-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8880-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8880-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

## <a name="request-headers"></a><span data-ttu-id="a8880-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8880-118">Request headers</span></span>

|<span data-ttu-id="a8880-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a8880-119">Name</span></span>|<span data-ttu-id="a8880-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8880-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a8880-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8880-121">Authorization</span></span>|<span data-ttu-id="a8880-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8880-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8880-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8880-124">Request body</span></span>

<span data-ttu-id="a8880-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8880-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8880-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8880-126">Response</span></span>

<span data-ttu-id="a8880-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a8880-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a8880-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8880-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8880-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8880-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a8880-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8880-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```
# <a name="c"></a>[<span data-ttu-id="a8880-131">C#</span><span class="sxs-lookup"><span data-stu-id="a8880-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8880-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8880-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8880-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8880-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8880-134">Java</span><span class="sxs-lookup"><span data-stu-id="a8880-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8880-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8880-135">Response</span></span>

<span data-ttu-id="a8880-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a8880-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
