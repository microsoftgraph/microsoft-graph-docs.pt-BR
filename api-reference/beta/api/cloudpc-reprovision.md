---
title: 'cloudPC: reprovision'
description: Reprovisione um computador de nuvem específico.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 97c80333b61bed09e3747e7732ab778810b0c7fd
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546865"
---
# <a name="cloudpc-reprovision"></a><span data-ttu-id="c617a-103">cloudPC: reprovision</span><span class="sxs-lookup"><span data-stu-id="c617a-103">cloudPC: reprovision</span></span>

<span data-ttu-id="c617a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c617a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c617a-105">Reprovisione um computador de nuvem específico.</span><span class="sxs-lookup"><span data-stu-id="c617a-105">Reprovision a specific cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="c617a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c617a-106">Permissions</span></span>

<span data-ttu-id="c617a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c617a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c617a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c617a-109">Permission type</span></span>|<span data-ttu-id="c617a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c617a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c617a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c617a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c617a-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c617a-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="c617a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c617a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c617a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c617a-114">Not supported.</span></span>|
|<span data-ttu-id="c617a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c617a-115">Application</span></span>|<span data-ttu-id="c617a-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c617a-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c617a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c617a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

## <a name="request-headers"></a><span data-ttu-id="c617a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c617a-118">Request headers</span></span>

|<span data-ttu-id="c617a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c617a-119">Name</span></span>|<span data-ttu-id="c617a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c617a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c617a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c617a-121">Authorization</span></span>|<span data-ttu-id="c617a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c617a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c617a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c617a-124">Request body</span></span>

<span data-ttu-id="c617a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c617a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c617a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c617a-126">Response</span></span>

<span data-ttu-id="c617a-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c617a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c617a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c617a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c617a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c617a-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c617a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c617a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck_1"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```
# <a name="c"></a>[<span data-ttu-id="c617a-131">C#</span><span class="sxs-lookup"><span data-stu-id="c617a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpconpremisesconnection-runhealthcheck-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c617a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c617a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-runhealthcheck-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c617a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c617a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-runhealthcheck-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c617a-134">Java</span><span class="sxs-lookup"><span data-stu-id="c617a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpconpremisesconnection-runhealthcheck-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c617a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c617a-135">Response</span></span>

<span data-ttu-id="c617a-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c617a-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
