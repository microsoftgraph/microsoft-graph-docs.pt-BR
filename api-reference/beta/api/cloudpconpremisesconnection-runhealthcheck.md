---
title: CloudPcOnPremisesConnection-RunHealthChecks
description: Executar verificações de integridade na conexão local do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 484d48f0400c328090d66bbcf7a930a485a9d950
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378209"
---
# <a name="cloudpconpremisesconnection-runhealthchecks"></a><span data-ttu-id="9316c-103">CloudPcOnPremisesConnection: runHealthChecks</span><span class="sxs-lookup"><span data-stu-id="9316c-103">CloudPcOnPremisesConnection: runHealthChecks</span></span>

<span data-ttu-id="9316c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9316c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9316c-105">Executar verificações de integridade no objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="9316c-105">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="9316c-106">Isso disparará uma nova verificação de integridade para este objeto [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) e alterará as propriedades HealthCheckStatus e [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) quando o check for concluído.</span><span class="sxs-lookup"><span data-stu-id="9316c-106">This will trigger a new health check for this [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object and change the healthCheckStatus and [healthCheckStatusDetails](../resources/cloudpconpremisesconnectionstatusdetails.md) properties when check finished.</span></span>

## <a name="permissions"></a><span data-ttu-id="9316c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9316c-107">Permissions</span></span>

<span data-ttu-id="9316c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9316c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9316c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9316c-110">Permission type</span></span>|<span data-ttu-id="9316c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9316c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9316c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9316c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9316c-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9316c-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="9316c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9316c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9316c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9316c-115">Not supported.</span></span>|
|<span data-ttu-id="9316c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9316c-116">Application</span></span>|<span data-ttu-id="9316c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9316c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9316c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9316c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

## <a name="request-headers"></a><span data-ttu-id="9316c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9316c-119">Request headers</span></span>

|<span data-ttu-id="9316c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9316c-120">Name</span></span>|<span data-ttu-id="9316c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9316c-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9316c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9316c-122">Authorization</span></span>|<span data-ttu-id="9316c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9316c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9316c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9316c-125">Request body</span></span>

<span data-ttu-id="9316c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9316c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9316c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9316c-127">Response</span></span>

<span data-ttu-id="9316c-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9316c-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9316c-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9316c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9316c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9316c-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks
```

### <a name="response"></a><span data-ttu-id="9316c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9316c-131">Response</span></span>

<span data-ttu-id="9316c-132">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9316c-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
