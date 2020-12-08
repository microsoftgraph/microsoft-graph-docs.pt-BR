---
title: 'identityUserFlowAttributeAssignment: SetOrder'
description: Definir a ordem de identityUserFlowAttributeAssignments que está sendo coletada dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 705acf8e65d7d01c40d98860c6f5066121d23a81
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581297"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="ae3e2-103">identityUserFlowAttributeAssignment: SetOrder</span><span class="sxs-lookup"><span data-stu-id="ae3e2-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="ae3e2-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ae3e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae3e2-105">Definir a ordem de identityUserFlowAttributeAssignments que está sendo coletada dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="ae3e2-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae3e2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ae3e2-106">Permissions</span></span>

<span data-ttu-id="ae3e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae3e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae3e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae3e2-109">Permission type</span></span>|<span data-ttu-id="ae3e2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae3e2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae3e2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae3e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ae3e2-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ae3e2-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ae3e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae3e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae3e2-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ae3e2-114">Not supported</span></span>|
|<span data-ttu-id="ae3e2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae3e2-115">Application</span></span>|<span data-ttu-id="ae3e2-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ae3e2-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae3e2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae3e2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/setOrder
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="ae3e2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae3e2-118">Request headers</span></span>

|<span data-ttu-id="ae3e2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ae3e2-119">Name</span></span>|<span data-ttu-id="ae3e2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae3e2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ae3e2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae3e2-121">Authorization</span></span>|<span data-ttu-id="ae3e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae3e2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ae3e2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae3e2-124">Content-Type</span></span>|<span data-ttu-id="ae3e2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae3e2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae3e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae3e2-127">Request body</span></span>

<span data-ttu-id="ae3e2-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ae3e2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ae3e2-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ae3e2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ae3e2-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ae3e2-130">Parameter</span></span>|<span data-ttu-id="ae3e2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae3e2-131">Type</span></span>|<span data-ttu-id="ae3e2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae3e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae3e2-133">newAssignmentOrder</span><span class="sxs-lookup"><span data-stu-id="ae3e2-133">newAssignmentOrder</span></span>|[<span data-ttu-id="ae3e2-134">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="ae3e2-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="ae3e2-135">Usado para definir a ordem dos atributos que estão sendo coletados dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="ae3e2-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="ae3e2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae3e2-136">Response</span></span>

<span data-ttu-id="ae3e2-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ae3e2-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ae3e2-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ae3e2-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae3e2-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae3e2-139">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="ae3e2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae3e2-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
