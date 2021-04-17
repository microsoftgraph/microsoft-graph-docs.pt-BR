---
title: 'identityUserFlowAttributeAssignment: setOrder'
description: Definir a ordem de identityUserFlowAttributeAssignments sendo coletados em um fluxo de usuários.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2f066bc84a2938734776c4271022cb4756ac1620
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882745"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="4720d-103">identityUserFlowAttributeAssignment: setOrder</span><span class="sxs-lookup"><span data-stu-id="4720d-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="4720d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4720d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4720d-105">Definir a ordem de identityUserFlowAttributeAssignments sendo coletados em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="4720d-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="4720d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4720d-106">Permissions</span></span>

<span data-ttu-id="4720d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4720d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4720d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4720d-109">Permission type</span></span>|<span data-ttu-id="4720d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4720d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4720d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4720d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4720d-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4720d-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4720d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4720d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4720d-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4720d-114">Not supported</span></span>|
|<span data-ttu-id="4720d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4720d-115">Application</span></span>|<span data-ttu-id="4720d-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4720d-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4720d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4720d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="4720d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4720d-118">Request headers</span></span>

|<span data-ttu-id="4720d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4720d-119">Name</span></span>|<span data-ttu-id="4720d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4720d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4720d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4720d-121">Authorization</span></span>|<span data-ttu-id="4720d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4720d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4720d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4720d-124">Content-Type</span></span>|<span data-ttu-id="4720d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4720d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4720d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4720d-127">Request body</span></span>

<span data-ttu-id="4720d-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4720d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4720d-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="4720d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4720d-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4720d-130">Parameter</span></span>|<span data-ttu-id="4720d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4720d-131">Type</span></span>|<span data-ttu-id="4720d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4720d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4720d-133">newAssignmentOrder</span><span class="sxs-lookup"><span data-stu-id="4720d-133">newAssignmentOrder</span></span>|[<span data-ttu-id="4720d-134">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="4720d-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="4720d-135">Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4720d-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="4720d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4720d-136">Response</span></span>

<span data-ttu-id="4720d-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4720d-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4720d-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4720d-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4720d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4720d-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_setorder"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/userAttributeAssignments/setOrder
Content-Type: application/json
Content-length: 90

{
  "newAssignmentOrder": {
    "order": [
        "City",
        "extension_GUID_ShoeSize"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="4720d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4720d-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
