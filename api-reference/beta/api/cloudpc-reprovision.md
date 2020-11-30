---
title: 'cloudPC: reprovisionar'
description: Reconfigurar um PC de nuvem específico.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 33a467fad7368750fda2dd814c414ed01961ecc4
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378228"
---
# <a name="cloudpc-reprovision"></a><span data-ttu-id="065d4-103">cloudPC: reprovisionar</span><span class="sxs-lookup"><span data-stu-id="065d4-103">cloudPC: reprovision</span></span>

<span data-ttu-id="065d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="065d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="065d4-105">Reconfigurar um PC de nuvem específico.</span><span class="sxs-lookup"><span data-stu-id="065d4-105">Reprovision a specific cloud PC.</span></span>

## <a name="permissions"></a><span data-ttu-id="065d4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="065d4-106">Permissions</span></span>

<span data-ttu-id="065d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="065d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="065d4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="065d4-109">Permission type</span></span>|<span data-ttu-id="065d4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="065d4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="065d4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="065d4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="065d4-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="065d4-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="065d4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="065d4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="065d4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="065d4-114">Not supported.</span></span>|
|<span data-ttu-id="065d4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="065d4-115">Application</span></span>|<span data-ttu-id="065d4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="065d4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="065d4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="065d4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

## <a name="request-headers"></a><span data-ttu-id="065d4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="065d4-118">Request headers</span></span>

|<span data-ttu-id="065d4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="065d4-119">Name</span></span>|<span data-ttu-id="065d4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="065d4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="065d4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="065d4-121">Authorization</span></span>|<span data-ttu-id="065d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="065d4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="065d4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="065d4-124">Request body</span></span>

<span data-ttu-id="065d4-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="065d4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="065d4-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="065d4-126">Response</span></span>

<span data-ttu-id="065d4-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="065d4-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="065d4-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="065d4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="065d4-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="065d4-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_runhealthcheck"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}/reprovision
```

### <a name="response"></a><span data-ttu-id="065d4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="065d4-130">Response</span></span>

<span data-ttu-id="065d4-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="065d4-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
