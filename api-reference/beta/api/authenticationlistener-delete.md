---
title: Excluir authenticationListener
description: Exclui um authenticationListener de um evento suportado por um authenticationEventsPolicy.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cb6c12bbba8d5b458ed2dbf6829a88d8e0885e2b
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720054"
---
# <a name="remove-authenticationlistener"></a><span data-ttu-id="87ccf-103">Remover authenticationListener</span><span class="sxs-lookup"><span data-stu-id="87ccf-103">Remove authenticationListener</span></span>

<span data-ttu-id="87ccf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87ccf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87ccf-105">Exclua o [authenticationListener](../resources/authenticationlistener.md) especificado definido para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="87ccf-105">Delete the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="87ccf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87ccf-106">Permissions</span></span>

<span data-ttu-id="87ccf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87ccf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87ccf-109">Permission type</span></span>|<span data-ttu-id="87ccf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87ccf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87ccf-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87ccf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87ccf-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="87ccf-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="87ccf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87ccf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87ccf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87ccf-114">Not supported.</span></span>|
|<span data-ttu-id="87ccf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87ccf-115">Application</span></span>|<span data-ttu-id="87ccf-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="87ccf-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="87ccf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87ccf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="87ccf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87ccf-118">Request headers</span></span>

|<span data-ttu-id="87ccf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="87ccf-119">Name</span></span>|<span data-ttu-id="87ccf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="87ccf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="87ccf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="87ccf-121">Authorization</span></span>|<span data-ttu-id="87ccf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87ccf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87ccf-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87ccf-124">Request body</span></span>

<span data-ttu-id="87ccf-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87ccf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87ccf-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="87ccf-126">Response</span></span>

<span data-ttu-id="87ccf-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="87ccf-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="87ccf-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="87ccf-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="87ccf-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87ccf-129">Request</span></span>

<span data-ttu-id="87ccf-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87ccf-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onsignupstart_from_authenticationeventspolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

### <a name="response"></a><span data-ttu-id="87ccf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="87ccf-131">Response</span></span>

<span data-ttu-id="87ccf-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87ccf-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
