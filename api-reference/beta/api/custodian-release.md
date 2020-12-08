---
title: 'responsáveis: lançamento'
description: Liberar um dos casos.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 59e3ef5721c10419261443ca57d7584035dc1622
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597477"
---
# <a name="custodian-release"></a><span data-ttu-id="b52f0-103">responsáveis: lançamento</span><span class="sxs-lookup"><span data-stu-id="b52f0-103">custodian: release</span></span>

<span data-ttu-id="b52f0-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b52f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b52f0-105">Liberar um dos casos.</span><span class="sxs-lookup"><span data-stu-id="b52f0-105">Release a custodian from a case.</span></span> <span data-ttu-id="b52f0-106">Para obter detalhes, consulte [liberar um dos responsáveis por um caso](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span><span class="sxs-lookup"><span data-stu-id="b52f0-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="b52f0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="b52f0-107">Permissions</span></span>

<span data-ttu-id="b52f0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b52f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b52f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b52f0-110">Permission type</span></span>|<span data-ttu-id="b52f0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b52f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b52f0-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b52f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b52f0-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="b52f0-113">User.Read</span></span>|
|<span data-ttu-id="b52f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b52f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b52f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b52f0-115">Not supported.</span></span>|
|<span data-ttu-id="b52f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b52f0-116">Application</span></span>|<span data-ttu-id="b52f0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b52f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b52f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b52f0-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/release
```

## <a name="request-headers"></a><span data-ttu-id="b52f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b52f0-119">Request headers</span></span>

|<span data-ttu-id="b52f0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b52f0-120">Name</span></span>|<span data-ttu-id="b52f0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b52f0-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b52f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b52f0-122">Authorization</span></span>|<span data-ttu-id="b52f0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b52f0-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b52f0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b52f0-125">Content-Type</span></span>|<span data-ttu-id="b52f0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b52f0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b52f0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b52f0-128">Request body</span></span>

<span data-ttu-id="b52f0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b52f0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b52f0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b52f0-130">Response</span></span>

<span data-ttu-id="b52f0-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b52f0-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b52f0-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b52f0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b52f0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b52f0-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "custodian_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/release
```

### <a name="response"></a><span data-ttu-id="b52f0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b52f0-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
