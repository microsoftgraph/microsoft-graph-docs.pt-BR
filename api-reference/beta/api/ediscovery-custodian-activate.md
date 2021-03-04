---
title: 'custodiatário: ativar'
description: Reativar um custodiante em um caso.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 82f79abee2fe7cc64ce7f4efb4f7c950a29b7b88
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445810"
---
# <a name="custodian-activate"></a><span data-ttu-id="ebd68-103">custodiatário: ativar</span><span class="sxs-lookup"><span data-stu-id="ebd68-103">custodian: activate</span></span>

<span data-ttu-id="ebd68-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ebd68-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebd68-105">Ative um custodiante que foi liberado de um caso para torná-los parte do caso novamente.</span><span class="sxs-lookup"><span data-stu-id="ebd68-105">Activate a custodian that has been released from a case to make them part of the case again.</span></span> <span data-ttu-id="ebd68-106">Para obter detalhes, [consulte Manage custodians in an Advanced eDiscovery case](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian).</span><span class="sxs-lookup"><span data-stu-id="ebd68-106">For details, see [Manage custodians in an Advanced eDiscovery case](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian).</span></span>

## <a name="permissions"></a><span data-ttu-id="ebd68-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebd68-107">Permissions</span></span>

<span data-ttu-id="ebd68-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebd68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebd68-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebd68-110">Permission type</span></span>|<span data-ttu-id="ebd68-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebd68-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebd68-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebd68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebd68-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebd68-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="ebd68-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebd68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebd68-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebd68-115">Not supported.</span></span>|
|<span data-ttu-id="ebd68-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebd68-116">Application</span></span>|<span data-ttu-id="ebd68-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebd68-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebd68-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebd68-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/activate
```

## <a name="request-headers"></a><span data-ttu-id="ebd68-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd68-119">Request headers</span></span>

|<span data-ttu-id="ebd68-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ebd68-120">Name</span></span>|<span data-ttu-id="ebd68-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebd68-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ebd68-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebd68-122">Authorization</span></span>|<span data-ttu-id="ebd68-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebd68-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ebd68-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebd68-125">Content-Type</span></span>|<span data-ttu-id="ebd68-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebd68-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebd68-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd68-128">Request body</span></span>

<span data-ttu-id="ebd68-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebd68-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebd68-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebd68-130">Response</span></span>

<span data-ttu-id="ebd68-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ebd68-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ebd68-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ebd68-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ebd68-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd68-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ebd68-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebd68-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "custodian_activate"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/activate
```
# <a name="c"></a>[<span data-ttu-id="ebd68-135">C#</span><span class="sxs-lookup"><span data-stu-id="ebd68-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/custodian-activate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebd68-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebd68-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/custodian-activate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebd68-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebd68-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/custodian-activate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebd68-138">Java</span><span class="sxs-lookup"><span data-stu-id="ebd68-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/custodian-activate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ebd68-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebd68-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
