---
title: Excluir cloudPcProvisioningPolicy
description: Excluir um objeto cloudPcProvisioningPolicy.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 4f85b29e0375c10f8e3bb9f1132bf7c9a8b0aafd
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378238"
---
# <a name="delete-cloudpcprovisioningpolicy"></a><span data-ttu-id="b43d9-103">Excluir cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="b43d9-103">Delete cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="b43d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b43d9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b43d9-105">Excluir um objeto [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b43d9-105">Delete a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span> <span data-ttu-id="b43d9-106">Você não poderá excluir uma política que estiver em uso.</span><span class="sxs-lookup"><span data-stu-id="b43d9-106">You can’t delete a policy that’s in use.</span></span>

## <a name="permissions"></a><span data-ttu-id="b43d9-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="b43d9-107">Permissions</span></span>

<span data-ttu-id="b43d9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b43d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b43d9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b43d9-110">Permission type</span></span>|<span data-ttu-id="b43d9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b43d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b43d9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b43d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b43d9-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b43d9-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="b43d9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b43d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b43d9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b43d9-115">Not supported.</span></span>|
|<span data-ttu-id="b43d9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b43d9-116">Application</span></span>|<span data-ttu-id="b43d9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b43d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b43d9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b43d9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b43d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b43d9-119">Request headers</span></span>

|<span data-ttu-id="b43d9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b43d9-120">Name</span></span>|<span data-ttu-id="b43d9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b43d9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b43d9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b43d9-122">Authorization</span></span>|<span data-ttu-id="b43d9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b43d9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b43d9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b43d9-125">Request body</span></span>

<span data-ttu-id="b43d9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b43d9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b43d9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b43d9-127">Response</span></span>

<span data-ttu-id="b43d9-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b43d9-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b43d9-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b43d9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b43d9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b43d9-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_provisioningpolicies_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="b43d9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b43d9-131">Response</span></span>

<span data-ttu-id="b43d9-132">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b43d9-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
