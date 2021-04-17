---
title: 'identityUserFlowAttributeAssignment: getOrder'
description: Obter a ordem de identityUserFlowAttributeAssignments sendo coletados em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ea6e8aa4e5f27d0ae21b1ae593f045b29a5848af
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882767"
---
# <a name="identityuserflowattributeassignment-getorder"></a><span data-ttu-id="9482f-103">identityUserFlowAttributeAssignment: getOrder</span><span class="sxs-lookup"><span data-stu-id="9482f-103">identityUserFlowAttributeAssignment: getOrder</span></span>

<span data-ttu-id="9482f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9482f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9482f-105">Obter a ordem de identityUserFlowAttributeAssignments sendo coletados em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="9482f-105">Get the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="9482f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9482f-106">Permissions</span></span>

<span data-ttu-id="9482f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9482f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9482f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9482f-109">Permission type</span></span>|<span data-ttu-id="9482f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9482f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9482f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9482f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9482f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9482f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9482f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9482f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9482f-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9482f-114">Not supported</span></span>|
|<span data-ttu-id="9482f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9482f-115">Application</span></span>|<span data-ttu-id="9482f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9482f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9482f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9482f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/getOrder
```

## <a name="request-headers"></a><span data-ttu-id="9482f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9482f-118">Request headers</span></span>

|<span data-ttu-id="9482f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9482f-119">Name</span></span>|<span data-ttu-id="9482f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9482f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9482f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9482f-121">Authorization</span></span>|<span data-ttu-id="9482f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9482f-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="9482f-124">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9482f-124">Function parameters</span></span>

<span data-ttu-id="9482f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9482f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9482f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9482f-126">Response</span></span>

<span data-ttu-id="9482f-127">Se tiver êxito, essa função retornará um código `200 OK` de resposta e um [assignmentOrder](../resources/assignmentorder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9482f-127">If successful, this function returns a `200 OK` response code and a [assignmentOrder](../resources/assignmentorder.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9482f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9482f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9482f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9482f-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_getorder"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/getOrder
```

### <a name="response"></a><span data-ttu-id="9482f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9482f-130">Response</span></span>

<span data-ttu-id="9482f-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9482f-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta$metadata#microsoft.graph.assignmentOrder",
    "order": [
        "extension_GUID_ShoeSize",
        "City"
    ]
}
```
