---
title: 'ediscoveryCase: fechar'
description: Feche uma ocorrência de descoberta eletrônica.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 627c8c1547e8df03c6736f00a5cb571d1c8c93bb
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597505"
---
# <a name="ediscoverycase-close"></a><span data-ttu-id="73350-103">ediscoveryCase: fechar</span><span class="sxs-lookup"><span data-stu-id="73350-103">ediscoveryCase: close</span></span>

<span data-ttu-id="73350-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="73350-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73350-105">Feche uma ocorrência de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="73350-105">Close an eDiscovery case.</span></span> <span data-ttu-id="73350-106">Para obter detalhes, consulte [Close a Case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span><span class="sxs-lookup"><span data-stu-id="73350-106">For details, see [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="73350-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="73350-107">Permissions</span></span>

<span data-ttu-id="73350-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73350-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73350-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73350-110">Permission type</span></span>|<span data-ttu-id="73350-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73350-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73350-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73350-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73350-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="73350-113">User.Read</span></span>|
|<span data-ttu-id="73350-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73350-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73350-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73350-115">Not supported.</span></span>|
|<span data-ttu-id="73350-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73350-116">Application</span></span>|<span data-ttu-id="73350-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73350-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73350-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73350-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/close
```

## <a name="request-headers"></a><span data-ttu-id="73350-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73350-119">Request headers</span></span>

|<span data-ttu-id="73350-120">Nome</span><span class="sxs-lookup"><span data-stu-id="73350-120">Name</span></span>|<span data-ttu-id="73350-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="73350-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="73350-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73350-122">Authorization</span></span>|<span data-ttu-id="73350-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73350-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73350-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73350-125">Request body</span></span>

<span data-ttu-id="73350-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73350-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73350-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="73350-127">Response</span></span>

<span data-ttu-id="73350-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="73350-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="73350-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73350-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73350-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73350-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "ediscoverycase_close"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/close
```

### <a name="response"></a><span data-ttu-id="73350-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="73350-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
