---
title: Excluir usuário
description: Exclui um objeto username.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 150bf4eb1178b30dc1d76d4276a5164412255a6d
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597524"
---
# <a name="delete-usersource"></a><span data-ttu-id="def1c-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="def1c-103">Delete userSource</span></span>

<span data-ttu-id="def1c-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="def1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="def1c-105">Excluir um objeto [username](../resources/usersource.md) .</span><span class="sxs-lookup"><span data-stu-id="def1c-105">Delete a [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="def1c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="def1c-106">Permissions</span></span>

<span data-ttu-id="def1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="def1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="def1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="def1c-109">Permission type</span></span>|<span data-ttu-id="def1c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="def1c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="def1c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="def1c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="def1c-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="def1c-112">User.Read</span></span>|
|<span data-ttu-id="def1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="def1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="def1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="def1c-114">Not supported.</span></span>|
|<span data-ttu-id="def1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="def1c-115">Application</span></span>|<span data-ttu-id="def1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="def1c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="def1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="def1c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="def1c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="def1c-118">Request headers</span></span>

|<span data-ttu-id="def1c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="def1c-119">Name</span></span>|<span data-ttu-id="def1c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="def1c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="def1c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="def1c-121">Authorization</span></span>|<span data-ttu-id="def1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="def1c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="def1c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="def1c-124">Request body</span></span>

<span data-ttu-id="def1c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="def1c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="def1c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="def1c-126">Response</span></span>

<span data-ttu-id="def1c-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="def1c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="def1c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="def1c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="def1c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="def1c-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_usersource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```

### <a name="response"></a><span data-ttu-id="def1c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="def1c-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
