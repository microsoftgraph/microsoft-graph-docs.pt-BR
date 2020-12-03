---
title: Excluir cloudPcProvisioningPolicy
description: Excluir um objeto cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 18b98a3d7afab82e554b35a5dd018608407689a2
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563440"
---
# <a name="delete-cloudpcprovisioningpolicy"></a><span data-ttu-id="000e6-103">Excluir cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="000e6-103">Delete cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="000e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="000e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="000e6-105">Excluir um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="000e6-105">Delete a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span> <span data-ttu-id="000e6-106">Você não poderá excluir uma política que estiver em uso.</span><span class="sxs-lookup"><span data-stu-id="000e6-106">You can’t delete a policy that’s in use.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="000e6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="000e6-107">Permissions</span></span>

<span data-ttu-id="000e6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="000e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="000e6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="000e6-110">Permission type</span></span>|<span data-ttu-id="000e6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="000e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="000e6-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="000e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="000e6-113">CloudPC. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="000e6-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="000e6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="000e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="000e6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="000e6-115">Not supported.</span></span>|
|<span data-ttu-id="000e6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="000e6-116">Application</span></span>|<span data-ttu-id="000e6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="000e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="000e6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="000e6-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="000e6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="000e6-119">Request headers</span></span>

|<span data-ttu-id="000e6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="000e6-120">Name</span></span>|<span data-ttu-id="000e6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="000e6-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="000e6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="000e6-122">Authorization</span></span>|<span data-ttu-id="000e6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="000e6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="000e6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="000e6-125">Request body</span></span>

<span data-ttu-id="000e6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="000e6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="000e6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="000e6-127">Response</span></span>

<span data-ttu-id="000e6-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="000e6-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="000e6-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="000e6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="000e6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="000e6-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="000e6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="000e6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_provisioningpolicies_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="000e6-132">C#</span><span class="sxs-lookup"><span data-stu-id="000e6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-provisioningpolicies-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="000e6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="000e6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-provisioningpolicies-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="000e6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="000e6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-provisioningpolicies-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="000e6-135">Java</span><span class="sxs-lookup"><span data-stu-id="000e6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-provisioningpolicies-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="000e6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="000e6-136">Response</span></span>

<span data-ttu-id="000e6-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="000e6-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
