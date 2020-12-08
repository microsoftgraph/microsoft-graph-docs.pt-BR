---
title: 'identityUserFlowAttributeAssignment: GetOrder'
description: Obter a ordem de coleta de identityUserFlowAttributeAssignments em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 653a1e83ee96418dc70129790f62ea764e6326f9
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581296"
---
# <a name="identityuserflowattributeassignment-getorder"></a><span data-ttu-id="e7836-103">identityUserFlowAttributeAssignment: GetOrder</span><span class="sxs-lookup"><span data-stu-id="e7836-103">identityUserFlowAttributeAssignment: getOrder</span></span>

<span data-ttu-id="e7836-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e7836-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7836-105">Obter a ordem de coleta de identityUserFlowAttributeAssignments em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="e7836-105">Get the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7836-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e7836-106">Permissions</span></span>

<span data-ttu-id="e7836-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7836-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7836-109">Permission type</span></span>|<span data-ttu-id="e7836-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7836-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7836-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7836-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e7836-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e7836-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e7836-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7836-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7836-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e7836-114">Not supported</span></span>|
|<span data-ttu-id="e7836-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7836-115">Application</span></span>|<span data-ttu-id="e7836-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e7836-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7836-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7836-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/getOrder
GET /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/getOrder
```

## <a name="request-headers"></a><span data-ttu-id="e7836-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7836-118">Request headers</span></span>

|<span data-ttu-id="e7836-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e7836-119">Name</span></span>|<span data-ttu-id="e7836-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7836-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e7836-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7836-121">Authorization</span></span>|<span data-ttu-id="e7836-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7836-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="e7836-124">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e7836-124">Function parameters</span></span>

<span data-ttu-id="e7836-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7836-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7836-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7836-126">Response</span></span>

<span data-ttu-id="e7836-127">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [assignmentOrder](../resources/assignmentorder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7836-127">If successful, this function returns a `200 OK` response code and a [assignmentOrder](../resources/assignmentorder.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7836-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e7836-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7836-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7836-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_getorder"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder
```

### <a name="response"></a><span data-ttu-id="e7836-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7836-130">Response</span></span>

<span data-ttu-id="e7836-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e7836-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
