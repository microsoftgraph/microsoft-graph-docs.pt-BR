---
title: Excluir cloudPcOnPremisesConnection
description: Excluir um objeto cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 55e80278d76b36c7a0b17528878d4673a1626b5c
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563393"
---
# <a name="delete-cloudpconpremisesconnection"></a><span data-ttu-id="36571-103">Excluir cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="36571-103">Delete cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="36571-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36571-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36571-105">Excluir um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) específico.</span><span class="sxs-lookup"><span data-stu-id="36571-105">Delete a specific [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="36571-106">Quando você exclui uma conexão, as permissões para o serviço são removidas dos recursos do Azure especificados.</span><span class="sxs-lookup"><span data-stu-id="36571-106">When you delete a connection, permissions to the service are removed from the specified Azure resources.</span></span>

<span data-ttu-id="36571-107">Você não pode excluir uma conexão local depois que ela passa verificação de integridade, que é indicada pela `healthCheckStatus` propriedade.</span><span class="sxs-lookup"><span data-stu-id="36571-107">You cannot delete an on-premises connection once it passes health check, which is indicated by the `healthCheckStatus` property.</span></span>

<span data-ttu-id="36571-108">Não é possível excluir uma conexão quando ela está em uso, conforme indicado pela `inUse` propriedade.</span><span class="sxs-lookup"><span data-stu-id="36571-108">You cannot delete a connection when it's in use either, as indicated by the `inUse` property.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="36571-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="36571-109">Permissions</span></span>

<span data-ttu-id="36571-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36571-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36571-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36571-112">Permission type</span></span>|<span data-ttu-id="36571-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36571-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36571-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36571-114">Delegated (work or school account)</span></span>|<span data-ttu-id="36571-115">CloudPC. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="36571-115">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="36571-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36571-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36571-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36571-117">Not supported.</span></span>|
|<span data-ttu-id="36571-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36571-118">Application</span></span>|<span data-ttu-id="36571-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36571-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36571-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36571-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="36571-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36571-121">Request headers</span></span>

|<span data-ttu-id="36571-122">Nome</span><span class="sxs-lookup"><span data-stu-id="36571-122">Name</span></span>|<span data-ttu-id="36571-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="36571-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="36571-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="36571-124">Authorization</span></span>|<span data-ttu-id="36571-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36571-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36571-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36571-127">Request body</span></span>

<span data-ttu-id="36571-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36571-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36571-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="36571-129">Response</span></span>

<span data-ttu-id="36571-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="36571-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="36571-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36571-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36571-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36571-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36571-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="36571-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesconnections_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="36571-134">C#</span><span class="sxs-lookup"><span data-stu-id="36571-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesconnections-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36571-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36571-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesconnections-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36571-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36571-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesconnections-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36571-137">Java</span><span class="sxs-lookup"><span data-stu-id="36571-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-onpremisesconnections-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36571-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="36571-138">Response</span></span>

<span data-ttu-id="36571-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36571-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
