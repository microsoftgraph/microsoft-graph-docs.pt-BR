---
title: 'custodian: release'
description: Libere um custodiante de um caso.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: baf0eb188e0419ca5b7a34e8274515b47d3daafd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445797"
---
# <a name="custodian-release"></a><span data-ttu-id="f8179-103">custodian: release</span><span class="sxs-lookup"><span data-stu-id="f8179-103">custodian: release</span></span>

<span data-ttu-id="f8179-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f8179-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8179-105">Libere um custodiante de um caso.</span><span class="sxs-lookup"><span data-stu-id="f8179-105">Release a custodian from a case.</span></span> <span data-ttu-id="f8179-106">Para obter detalhes, [consulte Liberar um custodiante de um caso](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span><span class="sxs-lookup"><span data-stu-id="f8179-106">For details, see [Release a custodian from a case](/microsoft-365/compliance/manage-new-custodians#release-a-custodian-from-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8179-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8179-107">Permissions</span></span>

<span data-ttu-id="f8179-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8179-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8179-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8179-110">Permission type</span></span>|<span data-ttu-id="f8179-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8179-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8179-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8179-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8179-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8179-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f8179-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8179-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8179-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8179-115">Not supported.</span></span>|
|<span data-ttu-id="f8179-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8179-116">Application</span></span>|<span data-ttu-id="f8179-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8179-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8179-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8179-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/release
```

## <a name="request-headers"></a><span data-ttu-id="f8179-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8179-119">Request headers</span></span>

|<span data-ttu-id="f8179-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f8179-120">Name</span></span>|<span data-ttu-id="f8179-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8179-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8179-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8179-122">Authorization</span></span>|<span data-ttu-id="f8179-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8179-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f8179-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8179-125">Content-Type</span></span>|<span data-ttu-id="f8179-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8179-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8179-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8179-128">Request body</span></span>

<span data-ttu-id="f8179-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8179-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8179-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8179-130">Response</span></span>

<span data-ttu-id="f8179-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f8179-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f8179-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f8179-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8179-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8179-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f8179-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8179-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "custodian_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/release
```
# <a name="c"></a>[<span data-ttu-id="f8179-135">C#</span><span class="sxs-lookup"><span data-stu-id="f8179-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/custodian-release-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8179-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8179-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/custodian-release-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8179-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8179-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/custodian-release-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8179-138">Java</span><span class="sxs-lookup"><span data-stu-id="f8179-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/custodian-release-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8179-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8179-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
