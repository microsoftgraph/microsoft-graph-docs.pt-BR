---
title: 'unifiedRoleEligibilityScheduleRequest: cancel'
description: Cancele um unifiedRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c877c30ed016a83a9c1da8019a33467e232fc110
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680084"
---
# <a name="unifiedroleeligibilityschedulerequest-cancel"></a><span data-ttu-id="5d26d-103">unifiedRoleEligibilityScheduleRequest: cancel</span><span class="sxs-lookup"><span data-stu-id="5d26d-103">unifiedRoleEligibilityScheduleRequest: cancel</span></span>
<span data-ttu-id="5d26d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d26d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d26d-105">Cancele imediatamente [um unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e o sistema exclua automaticamente a solicitação cancelada após 30 dias.</span><span class="sxs-lookup"><span data-stu-id="5d26d-105">Immediately cancel a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d26d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d26d-106">Permissions</span></span>
<span data-ttu-id="5d26d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d26d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d26d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d26d-109">Permission type</span></span>|<span data-ttu-id="5d26d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d26d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d26d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d26d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5d26d-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="5d26d-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="5d26d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d26d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d26d-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5d26d-114">Not supported</span></span>|
|<span data-ttu-id="5d26d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d26d-115">Application</span></span>|<span data-ttu-id="5d26d-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5d26d-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d26d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d26d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="5d26d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d26d-118">Request headers</span></span>
|<span data-ttu-id="5d26d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5d26d-119">Name</span></span>|<span data-ttu-id="5d26d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d26d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5d26d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d26d-121">Authorization</span></span>|<span data-ttu-id="5d26d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d26d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d26d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d26d-124">Request body</span></span>
<span data-ttu-id="5d26d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d26d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d26d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d26d-126">Response</span></span>

<span data-ttu-id="5d26d-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5d26d-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5d26d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5d26d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d26d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d26d-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5d26d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d26d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="5d26d-131">C#</span><span class="sxs-lookup"><span data-stu-id="5d26d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleeligibilityschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d26d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d26d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleeligibilityschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d26d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d26d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleeligibilityschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d26d-134">Java</span><span class="sxs-lookup"><span data-stu-id="5d26d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleeligibilityschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5d26d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d26d-135">Response</span></span>
<span data-ttu-id="5d26d-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5d26d-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

