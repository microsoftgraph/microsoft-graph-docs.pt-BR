---
title: Excluir userAttributeAssignment
description: Exclua um objeto identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2cf34a4e1da47a0c974585f430fa0d3f85dcf552
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882803"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="57e17-103">Excluir userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="57e17-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="57e17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57e17-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57e17-105">[Exclua um objeto identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="57e17-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57e17-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="57e17-106">Permissions</span></span>

<span data-ttu-id="57e17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57e17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57e17-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57e17-109">Permission type</span></span>|<span data-ttu-id="57e17-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57e17-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57e17-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57e17-111">Delegated (work or school account)</span></span>|<span data-ttu-id="57e17-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57e17-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="57e17-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57e17-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57e17-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="57e17-114">Not supported</span></span>|
|<span data-ttu-id="57e17-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57e17-115">Application</span></span>|<span data-ttu-id="57e17-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57e17-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57e17-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57e17-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="57e17-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57e17-118">Request headers</span></span>

|<span data-ttu-id="57e17-119">Nome</span><span class="sxs-lookup"><span data-stu-id="57e17-119">Name</span></span>|<span data-ttu-id="57e17-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="57e17-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="57e17-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="57e17-121">Authorization</span></span>|<span data-ttu-id="57e17-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57e17-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57e17-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57e17-124">Request body</span></span>

<span data-ttu-id="57e17-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57e17-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57e17-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="57e17-126">Response</span></span>

<span data-ttu-id="57e17-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57e17-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="57e17-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="57e17-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57e17-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57e17-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2xidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City
```

### <a name="response"></a><span data-ttu-id="57e17-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="57e17-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
