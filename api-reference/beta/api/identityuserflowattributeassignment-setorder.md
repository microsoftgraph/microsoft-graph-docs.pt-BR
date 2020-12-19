---
title: 'identityUserFlowAttributeAssignment: SetOrder'
description: Definir a ordem de identityUserFlowAttributeAssignments que está sendo coletada dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5f1235987a0c9f90f5d5bd969cad7a20fb185a26
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719934"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="cebbc-103">identityUserFlowAttributeAssignment: SetOrder</span><span class="sxs-lookup"><span data-stu-id="cebbc-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="cebbc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cebbc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cebbc-105">Definir a ordem de identityUserFlowAttributeAssignments que está sendo coletada dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="cebbc-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="cebbc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cebbc-106">Permissions</span></span>

<span data-ttu-id="cebbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cebbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cebbc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cebbc-109">Permission type</span></span>|<span data-ttu-id="cebbc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cebbc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cebbc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cebbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cebbc-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebbc-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="cebbc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cebbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cebbc-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cebbc-114">Not supported</span></span>|
|<span data-ttu-id="cebbc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cebbc-115">Application</span></span>|<span data-ttu-id="cebbc-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cebbc-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cebbc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cebbc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/setOrder
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="cebbc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cebbc-118">Request headers</span></span>

|<span data-ttu-id="cebbc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cebbc-119">Name</span></span>|<span data-ttu-id="cebbc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cebbc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cebbc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cebbc-121">Authorization</span></span>|<span data-ttu-id="cebbc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cebbc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cebbc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cebbc-124">Content-Type</span></span>|<span data-ttu-id="cebbc-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cebbc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cebbc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cebbc-127">Request body</span></span>

<span data-ttu-id="cebbc-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="cebbc-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cebbc-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="cebbc-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cebbc-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cebbc-130">Parameter</span></span>|<span data-ttu-id="cebbc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cebbc-131">Type</span></span>|<span data-ttu-id="cebbc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cebbc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cebbc-133">newAssignmentOrder</span><span class="sxs-lookup"><span data-stu-id="cebbc-133">newAssignmentOrder</span></span>|[<span data-ttu-id="cebbc-134">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="cebbc-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="cebbc-135">Usado para definir a ordem dos atributos que estão sendo coletados dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="cebbc-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="cebbc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cebbc-136">Response</span></span>

<span data-ttu-id="cebbc-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cebbc-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cebbc-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cebbc-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cebbc-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cebbc-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cebbc-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="cebbc-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_setorder"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/setOrder
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
# <a name="javascript"></a>[<span data-ttu-id="cebbc-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cebbc-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityuserflowattributeassignment-setorder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cebbc-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cebbc-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
