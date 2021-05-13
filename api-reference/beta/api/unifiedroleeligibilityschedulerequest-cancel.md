---
title: 'unifiedRoleEligibilityScheduleRequest: cancel'
description: Cancele um unifiedRoleEligibilityScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 325eb611042cf4627cb1a02f15fad8513ba70870
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474453"
---
# <a name="unifiedroleeligibilityschedulerequest-cancel"></a><span data-ttu-id="fb68a-103">unifiedRoleEligibilityScheduleRequest: cancel</span><span class="sxs-lookup"><span data-stu-id="fb68a-103">unifiedRoleEligibilityScheduleRequest: cancel</span></span>
<span data-ttu-id="fb68a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb68a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb68a-105">Cancele imediatamente [um unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) e o sistema exclua automaticamente a solicitação cancelada após 30 dias.</span><span class="sxs-lookup"><span data-stu-id="fb68a-105">Immediately cancel a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb68a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb68a-106">Permissions</span></span>
<span data-ttu-id="fb68a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb68a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb68a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb68a-109">Permission type</span></span>|<span data-ttu-id="fb68a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb68a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb68a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb68a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb68a-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="fb68a-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="fb68a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb68a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb68a-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fb68a-114">Not supported</span></span>|
|<span data-ttu-id="fb68a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb68a-115">Application</span></span>|<span data-ttu-id="fb68a-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fb68a-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb68a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb68a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="fb68a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb68a-118">Request headers</span></span>
|<span data-ttu-id="fb68a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fb68a-119">Name</span></span>|<span data-ttu-id="fb68a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb68a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fb68a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb68a-121">Authorization</span></span>|<span data-ttu-id="fb68a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb68a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb68a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb68a-124">Request body</span></span>
<span data-ttu-id="fb68a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fb68a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb68a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb68a-126">Response</span></span>

<span data-ttu-id="fb68a-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb68a-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="fb68a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb68a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb68a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb68a-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fb68a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb68a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="fb68a-131">C#</span><span class="sxs-lookup"><span data-stu-id="fb68a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleeligibilityschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb68a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb68a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleeligibilityschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb68a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb68a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleeligibilityschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb68a-134">Java</span><span class="sxs-lookup"><span data-stu-id="fb68a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleeligibilityschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fb68a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb68a-135">Response</span></span>
<span data-ttu-id="fb68a-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb68a-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

