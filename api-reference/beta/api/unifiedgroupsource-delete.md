---
title: Excluir unifiedGroupSource
description: Excluir um objeto unifiedGroupSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 61e2eb86c566703e6c23262a0ddb572e438d33ce
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597528"
---
# <a name="delete-unifiedgroupsource"></a><span data-ttu-id="bc8ac-103">Excluir unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="bc8ac-103">Delete unifiedGroupSource</span></span>

<span data-ttu-id="bc8ac-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bc8ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc8ac-105">Excluir um objeto [unifiedGroupSource](../resources/unifiedgroupsource.md) .</span><span class="sxs-lookup"><span data-stu-id="bc8ac-105">Delete a [unifiedGroupSource](../resources/unifiedgroupsource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc8ac-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="bc8ac-106">Permissions</span></span>

<span data-ttu-id="bc8ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc8ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc8ac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc8ac-109">Permission type</span></span>|<span data-ttu-id="bc8ac-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bc8ac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc8ac-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc8ac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc8ac-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="bc8ac-112">User.Read</span></span>|
|<span data-ttu-id="bc8ac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc8ac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc8ac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc8ac-114">Not supported.</span></span>|
|<span data-ttu-id="bc8ac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc8ac-115">Application</span></span>|<span data-ttu-id="bc8ac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc8ac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc8ac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc8ac-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources/33434233-3030-3739-3043-393039324633
```

## <a name="request-headers"></a><span data-ttu-id="bc8ac-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc8ac-118">Request headers</span></span>

|<span data-ttu-id="bc8ac-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bc8ac-119">Name</span></span>|<span data-ttu-id="bc8ac-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc8ac-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bc8ac-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc8ac-121">Authorization</span></span>|<span data-ttu-id="bc8ac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc8ac-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc8ac-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc8ac-124">Request body</span></span>

<span data-ttu-id="bc8ac-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc8ac-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc8ac-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc8ac-126">Response</span></span>

<span data-ttu-id="bc8ac-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bc8ac-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bc8ac-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bc8ac-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bc8ac-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc8ac-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_unifiedgroupsource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources/{unifiedGroupSourceId}
```

### <a name="response"></a><span data-ttu-id="bc8ac-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc8ac-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
