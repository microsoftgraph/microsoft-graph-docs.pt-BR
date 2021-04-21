---
title: 'identityUserFlowAttributeAssignment: setOrder'
description: Definir a ordem de identityUserFlowAttributeAssignments sendo coletados em um fluxo de usuários.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dc9e539b56d44bcfedf5818b7be6126421fedd96
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920636"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="aacca-103">identityUserFlowAttributeAssignment: setOrder</span><span class="sxs-lookup"><span data-stu-id="aacca-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="aacca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aacca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aacca-105">Definir a ordem de identityUserFlowAttributeAssignments sendo coletados em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="aacca-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="aacca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aacca-106">Permissions</span></span>

<span data-ttu-id="aacca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aacca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aacca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aacca-109">Permission type</span></span>|<span data-ttu-id="aacca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aacca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aacca-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aacca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aacca-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacca-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="aacca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aacca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aacca-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aacca-114">Not supported</span></span>|
|<span data-ttu-id="aacca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aacca-115">Application</span></span>|<span data-ttu-id="aacca-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacca-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aacca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aacca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="aacca-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aacca-118">Request headers</span></span>

|<span data-ttu-id="aacca-119">Nome</span><span class="sxs-lookup"><span data-stu-id="aacca-119">Name</span></span>|<span data-ttu-id="aacca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="aacca-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aacca-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="aacca-121">Authorization</span></span>|<span data-ttu-id="aacca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aacca-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aacca-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aacca-124">Content-Type</span></span>|<span data-ttu-id="aacca-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aacca-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aacca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aacca-127">Request body</span></span>

<span data-ttu-id="aacca-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="aacca-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aacca-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="aacca-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aacca-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aacca-130">Parameter</span></span>|<span data-ttu-id="aacca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aacca-131">Type</span></span>|<span data-ttu-id="aacca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aacca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aacca-133">newAssignmentOrder</span><span class="sxs-lookup"><span data-stu-id="aacca-133">newAssignmentOrder</span></span>|[<span data-ttu-id="aacca-134">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="aacca-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="aacca-135">Usado para definir a ordem dos atributos que estão sendo coletados em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="aacca-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="aacca-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="aacca-136">Response</span></span>

<span data-ttu-id="aacca-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aacca-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="aacca-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aacca-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aacca-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aacca-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aacca-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="aacca-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="aacca-141">C#</span><span class="sxs-lookup"><span data-stu-id="aacca-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityuserflowattributeassignment-setorder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aacca-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aacca-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityuserflowattributeassignment-setorder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aacca-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aacca-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityuserflowattributeassignment-setorder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aacca-144">Java</span><span class="sxs-lookup"><span data-stu-id="aacca-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityuserflowattributeassignment-setorder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aacca-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="aacca-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
