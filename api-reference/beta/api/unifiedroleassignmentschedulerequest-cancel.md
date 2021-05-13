---
title: 'unifiedRoleAssignmentScheduleRequest: cancel'
description: Cancele um unifiedRoleAssignmentScheduleRequest.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c0e2f5dae3ae0b13bc6907d2ecb5560405c98c5b
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475090"
---
# <a name="unifiedroleassignmentschedulerequest-cancel"></a><span data-ttu-id="47fd8-103">unifiedRoleAssignmentScheduleRequest: cancel</span><span class="sxs-lookup"><span data-stu-id="47fd8-103">unifiedRoleAssignmentScheduleRequest: cancel</span></span>
<span data-ttu-id="47fd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47fd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47fd8-105">Cancele imediatamente [um unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) e o sistema exclua automaticamente a solicitação cancelada após 30 dias.</span><span class="sxs-lookup"><span data-stu-id="47fd8-105">Immediately cancel a [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="47fd8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47fd8-106">Permissions</span></span>
<span data-ttu-id="47fd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47fd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47fd8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47fd8-109">Permission type</span></span>|<span data-ttu-id="47fd8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47fd8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47fd8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47fd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47fd8-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="47fd8-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="47fd8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47fd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47fd8-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="47fd8-114">Not supported</span></span>|
|<span data-ttu-id="47fd8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47fd8-115">Application</span></span>|<span data-ttu-id="47fd8-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="47fd8-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="47fd8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47fd8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="47fd8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47fd8-118">Request headers</span></span>
|<span data-ttu-id="47fd8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="47fd8-119">Name</span></span>|<span data-ttu-id="47fd8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="47fd8-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47fd8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="47fd8-121">Authorization</span></span>|<span data-ttu-id="47fd8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47fd8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47fd8-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47fd8-124">Request body</span></span>
<span data-ttu-id="47fd8-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47fd8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47fd8-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="47fd8-126">Response</span></span>

<span data-ttu-id="47fd8-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="47fd8-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="47fd8-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47fd8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47fd8-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47fd8-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="47fd8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="47fd8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleassignmentschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="47fd8-131">C#</span><span class="sxs-lookup"><span data-stu-id="47fd8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleassignmentschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47fd8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47fd8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleassignmentschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47fd8-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47fd8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleassignmentschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47fd8-134">Java</span><span class="sxs-lookup"><span data-stu-id="47fd8-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleassignmentschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="47fd8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="47fd8-135">Response</span></span>
<span data-ttu-id="47fd8-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47fd8-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

