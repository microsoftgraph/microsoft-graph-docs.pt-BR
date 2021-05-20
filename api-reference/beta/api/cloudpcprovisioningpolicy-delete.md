---
title: Excluir cloudPcProvisioningPolicy
description: Exclua um objeto cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 8c423bdc23ec090b56bc096a797daeaed61bdcd0
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546816"
---
# <a name="delete-cloudpcprovisioningpolicy"></a><span data-ttu-id="0db18-103">Excluir cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="0db18-103">Delete cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="0db18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0db18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0db18-105">[Exclua um objeto cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0db18-105">Delete a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span> <span data-ttu-id="0db18-106">Você não poderá excluir uma política que estiver em uso.</span><span class="sxs-lookup"><span data-stu-id="0db18-106">You can’t delete a policy that’s in use.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="0db18-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0db18-107">Permissions</span></span>

<span data-ttu-id="0db18-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0db18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0db18-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0db18-110">Permission type</span></span>|<span data-ttu-id="0db18-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0db18-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0db18-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0db18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0db18-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db18-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="0db18-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0db18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0db18-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0db18-115">Not supported.</span></span>|
|<span data-ttu-id="0db18-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0db18-116">Application</span></span>|<span data-ttu-id="0db18-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db18-117">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0db18-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0db18-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0db18-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0db18-119">Request headers</span></span>

|<span data-ttu-id="0db18-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0db18-120">Name</span></span>|<span data-ttu-id="0db18-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0db18-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0db18-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0db18-122">Authorization</span></span>|<span data-ttu-id="0db18-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0db18-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0db18-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0db18-125">Request body</span></span>

<span data-ttu-id="0db18-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0db18-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0db18-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0db18-127">Response</span></span>

<span data-ttu-id="0db18-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0db18-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0db18-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0db18-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0db18-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0db18-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0db18-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0db18-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_provisioningpolicies_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="0db18-132">C#</span><span class="sxs-lookup"><span data-stu-id="0db18-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-provisioningpolicies-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0db18-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0db18-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-provisioningpolicies-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0db18-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0db18-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-provisioningpolicies-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0db18-135">Java</span><span class="sxs-lookup"><span data-stu-id="0db18-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-provisioningpolicies-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0db18-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0db18-136">Response</span></span>

<span data-ttu-id="0db18-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0db18-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
