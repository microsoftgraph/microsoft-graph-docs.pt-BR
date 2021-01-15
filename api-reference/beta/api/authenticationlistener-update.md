---
title: Atualizar authenticationListener
description: Atualize o ouvinte definido para um evento no pipeline de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5acb660843bf0b7a60fd66886841ab4c490f396
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872391"
---
# <a name="update-authenticationlistener"></a><span data-ttu-id="871dd-103">Atualizar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="871dd-103">Update authenticationListener</span></span>

<span data-ttu-id="871dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="871dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="871dd-105">Atualize [o authenticationListener definido](../resources/authenticationlistener.md) para um evento no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="871dd-105">Update the [authenticationListener](../resources/authenticationlistener.md) defined for an event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="871dd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="871dd-106">Permissions</span></span>

<span data-ttu-id="871dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="871dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="871dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="871dd-109">Permission type</span></span>|<span data-ttu-id="871dd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="871dd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="871dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="871dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="871dd-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="871dd-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="871dd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="871dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="871dd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="871dd-114">Not supported.</span></span>|
|<span data-ttu-id="871dd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="871dd-115">Application</span></span>|<span data-ttu-id="871dd-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="871dd-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="871dd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="871dd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="871dd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="871dd-118">Request headers</span></span>

|<span data-ttu-id="871dd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="871dd-119">Name</span></span>|<span data-ttu-id="871dd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="871dd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="871dd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="871dd-121">Authorization</span></span>|<span data-ttu-id="871dd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="871dd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="871dd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="871dd-124">Content-Type</span></span>|<span data-ttu-id="871dd-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="871dd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="871dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="871dd-127">Request body</span></span>

<span data-ttu-id="871dd-128">No corpo da solicitação, fornece uma representação JSON do [objeto authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="871dd-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="871dd-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [invokeUserFlowAction](../resources/invokeuserflowlistener.md).</span><span class="sxs-lookup"><span data-stu-id="871dd-129">The following table shows the properties that are required when you update the [invokeUserFlowAction](../resources/invokeuserflowlistener.md).</span></span>

|<span data-ttu-id="871dd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="871dd-130">Property</span></span>|<span data-ttu-id="871dd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="871dd-131">Type</span></span>|<span data-ttu-id="871dd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="871dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="871dd-133">Prioridade</span><span class="sxs-lookup"><span data-stu-id="871dd-133">priority</span></span>|<span data-ttu-id="871dd-134">Int32</span><span class="sxs-lookup"><span data-stu-id="871dd-134">Int32</span></span>|<span data-ttu-id="871dd-135">A prioridade do ouvinte.</span><span class="sxs-lookup"><span data-stu-id="871dd-135">The priority of the listener.</span></span> <span data-ttu-id="871dd-136">Determina a ordem de avaliação quando um evento tem vários ouvintes.</span><span class="sxs-lookup"><span data-stu-id="871dd-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="871dd-137">A prioridade é avaliada de baixo para alto.</span><span class="sxs-lookup"><span data-stu-id="871dd-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="871dd-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="871dd-138">sourceFilter</span></span>|[<span data-ttu-id="871dd-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="871dd-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="871dd-140">Filtrar com base na origem da autenticação que é usada para determinar se o ouvinte é avaliado.</span><span class="sxs-lookup"><span data-stu-id="871dd-140">Filter based on the source of the authentication which is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="871dd-141">Atualmente, isso está limitado a avaliações baseadas no aplicativo ao usuário que está autenticando.</span><span class="sxs-lookup"><span data-stu-id="871dd-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="response"></a><span data-ttu-id="871dd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="871dd-142">Response</span></span>

<span data-ttu-id="871dd-143">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="871dd-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="871dd-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="871dd-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="871dd-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="871dd-145">Request</span></span>

<span data-ttu-id="871dd-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="871dd-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_onsignupstart"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
Content-Type: application/json

{
  "priority": 101
}
```

### <a name="response"></a><span data-ttu-id="871dd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="871dd-147">Response</span></span>

<span data-ttu-id="871dd-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="871dd-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
