---
title: Excluir userAttributeAssignment
description: Excluir um objeto identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ea4c9ef7d2d9318c8b39b22dbdb72e43890d7dc2
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581298"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="9ab3c-103">Excluir userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="9ab3c-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="9ab3c-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9ab3c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ab3c-105">Excluir um objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9ab3c-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ab3c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9ab3c-106">Permissions</span></span>

<span data-ttu-id="9ab3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ab3c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ab3c-109">Permission type</span></span>|<span data-ttu-id="9ab3c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ab3c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ab3c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ab3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ab3c-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9ab3c-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9ab3c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ab3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ab3c-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9ab3c-114">Not supported</span></span>|
|<span data-ttu-id="9ab3c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ab3c-115">Application</span></span>|<span data-ttu-id="9ab3c-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9ab3c-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ab3c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab3c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9ab3c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab3c-118">Request headers</span></span>

|<span data-ttu-id="9ab3c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9ab3c-119">Name</span></span>|<span data-ttu-id="9ab3c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab3c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9ab3c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ab3c-121">Authorization</span></span>|<span data-ttu-id="9ab3c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ab3c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ab3c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab3c-124">Request body</span></span>

<span data-ttu-id="9ab3c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ab3c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ab3c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab3c-126">Response</span></span>

<span data-ttu-id="9ab3c-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9ab3c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9ab3c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9ab3c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ab3c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab3c-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2cidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```

### <a name="response"></a><span data-ttu-id="9ab3c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab3c-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
