---
title: Excluir cloudPcOnPremisesConnection
description: Excluir um objeto cloudPcOnPremisesConnection.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 73c3f899a3c7fbc862ddb68a243dbddd33205ba4
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378213"
---
# <a name="delete-cloudpconpremisesconnection"></a><span data-ttu-id="b45fc-103">Excluir cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="b45fc-103">Delete cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="b45fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b45fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b45fc-105">Excluir um objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) específico.</span><span class="sxs-lookup"><span data-stu-id="b45fc-105">Delete a specific [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="b45fc-106">Quando você exclui uma conexão, as permissões para o serviço são removidas dos recursos do Azure especificados.</span><span class="sxs-lookup"><span data-stu-id="b45fc-106">When you delete a connection, permissions to the service are removed from the specified Azure resources.</span></span>

<span data-ttu-id="b45fc-107">Você não pode excluir uma conexão local depois que ela passa verificação de integridade, que é indicada pela `healthCheckStatus` propriedade.</span><span class="sxs-lookup"><span data-stu-id="b45fc-107">You cannot delete an on-premises connection once it passes health check, which is indicated by the `healthCheckStatus` property.</span></span>

<span data-ttu-id="b45fc-108">Não é possível excluir uma conexão quando ela está em uso, conforme indicado pela `inUse` propriedade.</span><span class="sxs-lookup"><span data-stu-id="b45fc-108">You cannot delete a connection when it's in use either, as indicated by the `inUse` property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b45fc-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="b45fc-109">Permissions</span></span>

<span data-ttu-id="b45fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b45fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b45fc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b45fc-112">Permission type</span></span>|<span data-ttu-id="b45fc-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b45fc-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b45fc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b45fc-114">Delegated (work or school account)</span></span>|<span data-ttu-id="b45fc-115">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b45fc-115">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="b45fc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b45fc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b45fc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b45fc-117">Not supported.</span></span>|
|<span data-ttu-id="b45fc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b45fc-118">Application</span></span>|<span data-ttu-id="b45fc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b45fc-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b45fc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b45fc-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b45fc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b45fc-121">Request headers</span></span>

|<span data-ttu-id="b45fc-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b45fc-122">Name</span></span>|<span data-ttu-id="b45fc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b45fc-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b45fc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b45fc-124">Authorization</span></span>|<span data-ttu-id="b45fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b45fc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b45fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b45fc-127">Request body</span></span>

<span data-ttu-id="b45fc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b45fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b45fc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b45fc-129">Response</span></span>

<span data-ttu-id="b45fc-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b45fc-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b45fc-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b45fc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b45fc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b45fc-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onpremisesconnections_from_virtualendpoint"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

### <a name="response"></a><span data-ttu-id="b45fc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b45fc-133">Response</span></span>

<span data-ttu-id="b45fc-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b45fc-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
