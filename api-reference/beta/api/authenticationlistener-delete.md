---
title: Excluir authenticationListener
description: Exclui um authenticationListener de um evento suportado por uma authenticationEventsPolicy.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c808aa161bacb2612c90a53f58b7163f663e4150
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438488"
---
# <a name="remove-authenticationlistener"></a><span data-ttu-id="3942c-103">Remover authenticationListener</span><span class="sxs-lookup"><span data-stu-id="3942c-103">Remove authenticationListener</span></span>

<span data-ttu-id="3942c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3942c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3942c-105">Exclua a [autenticação especificadaListener definida](../resources/authenticationlistener.md) para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3942c-105">Delete the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="3942c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3942c-106">Permissions</span></span>

<span data-ttu-id="3942c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3942c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3942c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3942c-109">Permission type</span></span>|<span data-ttu-id="3942c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3942c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3942c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3942c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3942c-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3942c-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="3942c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3942c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3942c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3942c-114">Not supported.</span></span>|
|<span data-ttu-id="3942c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3942c-115">Application</span></span>|<span data-ttu-id="3942c-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="3942c-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="3942c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3942c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3942c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3942c-118">Request headers</span></span>

|<span data-ttu-id="3942c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3942c-119">Name</span></span>|<span data-ttu-id="3942c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3942c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3942c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3942c-121">Authorization</span></span>|<span data-ttu-id="3942c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3942c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3942c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3942c-124">Request body</span></span>

<span data-ttu-id="3942c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3942c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3942c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3942c-126">Response</span></span>

<span data-ttu-id="3942c-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3942c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3942c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3942c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3942c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3942c-129">Request</span></span>

<span data-ttu-id="3942c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3942c-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_onsignupstart_from_authenticationeventspolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

### <a name="response"></a><span data-ttu-id="3942c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3942c-131">Response</span></span>

<span data-ttu-id="3942c-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3942c-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
