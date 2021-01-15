---
title: Excluir cloudPcOnPremisesConnection
description: Exclua um objeto cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 01f9b5a7e4091492be7aa8eae0f0d3f8354169e6
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872762"
---
# <a name="delete-cloudpconpremisesconnection"></a><span data-ttu-id="4db2f-103">Excluir cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="4db2f-103">Delete cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="4db2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4db2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4db2f-105">[Exclua um objeto cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) específico.</span><span class="sxs-lookup"><span data-stu-id="4db2f-105">Delete a specific [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="4db2f-106">Quando você exclui uma conexão, as permissões para o serviço são removidas dos recursos especificados do Azure.</span><span class="sxs-lookup"><span data-stu-id="4db2f-106">When you delete a connection, permissions to the service are removed from the specified Azure resources.</span></span>

<span data-ttu-id="4db2f-107">Você não pode excluir uma conexão local depois que ela passar na verificação de saúde, que é indicada pela `healthCheckStatus` propriedade.</span><span class="sxs-lookup"><span data-stu-id="4db2f-107">You cannot delete an on-premises connection once it passes health check, which is indicated by the `healthCheckStatus` property.</span></span>

<span data-ttu-id="4db2f-108">Você também não pode excluir uma conexão quando ela está em uso, conforme indicado pela `inUse` propriedade.</span><span class="sxs-lookup"><span data-stu-id="4db2f-108">You cannot delete a connection when it's in use either, as indicated by the `inUse` property.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="4db2f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4db2f-109">Permissions</span></span>

<span data-ttu-id="4db2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4db2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4db2f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4db2f-112">Permission type</span></span>|<span data-ttu-id="4db2f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4db2f-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4db2f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4db2f-114">Delegated (work or school account)</span></span>|<span data-ttu-id="4db2f-115">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db2f-115">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="4db2f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4db2f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4db2f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4db2f-117">Not supported.</span></span>|
|<span data-ttu-id="4db2f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4db2f-118">Application</span></span>|<span data-ttu-id="4db2f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4db2f-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4db2f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4db2f-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4db2f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4db2f-121">Request headers</span></span>

|<span data-ttu-id="4db2f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4db2f-122">Name</span></span>|<span data-ttu-id="4db2f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4db2f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4db2f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4db2f-124">Authorization</span></span>|<span data-ttu-id="4db2f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4db2f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4db2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4db2f-127">Request body</span></span>

<span data-ttu-id="4db2f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4db2f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4db2f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4db2f-129">Response</span></span>

<span data-ttu-id="4db2f-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4db2f-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4db2f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4db2f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4db2f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4db2f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4db2f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4db2f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesconnections_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```
# <a name="c"></a>[<span data-ttu-id="4db2f-134">C#</span><span class="sxs-lookup"><span data-stu-id="4db2f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesconnections-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4db2f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4db2f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesconnections-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4db2f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4db2f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesconnections-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4db2f-137">Java</span><span class="sxs-lookup"><span data-stu-id="4db2f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-onpremisesconnections-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4db2f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4db2f-138">Response</span></span>

<span data-ttu-id="4db2f-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4db2f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
