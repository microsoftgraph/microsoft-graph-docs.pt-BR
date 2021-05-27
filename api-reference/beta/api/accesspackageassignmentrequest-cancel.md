---
title: 'accessPackageAssignmentRequest: cancel'
description: Cancele os objetos accessPackageAssignmentRequest que estão em estado cancelável.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 281eebc1008f8c1c791ac6cc2694a458c86f526b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679656"
---
# <a name="accesspackageassignmentrequest-cancel"></a><span data-ttu-id="15024-103">accessPackageAssignmentRequest: cancel</span><span class="sxs-lookup"><span data-stu-id="15024-103">accessPackageAssignmentRequest: cancel</span></span>
<span data-ttu-id="15024-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15024-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15024-105">No [Azure AD Entitlement Management,](../resources/entitlementmanagement-root.md)cancele os objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) que estão em estado cancelável: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .</span><span class="sxs-lookup"><span data-stu-id="15024-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), cancel [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects that are in a cancellable state: `accepted`, `pendingApproval`, `pendingNotBefore`, `pendingApprovalEscalated`.</span></span>

## <a name="permissions"></a><span data-ttu-id="15024-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="15024-106">Permissions</span></span>
<span data-ttu-id="15024-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15024-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15024-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15024-109">Permission type</span></span>|<span data-ttu-id="15024-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15024-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15024-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15024-111">Delegated (work or school account)</span></span>|<span data-ttu-id="15024-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15024-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="15024-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15024-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15024-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15024-114">Not supported.</span></span>|
|<span data-ttu-id="15024-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15024-115">Application</span></span>|<span data-ttu-id="15024-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15024-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15024-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15024-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="15024-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15024-118">Request headers</span></span>
|<span data-ttu-id="15024-119">Nome</span><span class="sxs-lookup"><span data-stu-id="15024-119">Name</span></span>|<span data-ttu-id="15024-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="15024-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="15024-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="15024-121">Authorization</span></span>|<span data-ttu-id="15024-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15024-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15024-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15024-124">Request body</span></span>
<span data-ttu-id="15024-125">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="15024-125">In the request body, supply a JSON representation of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="15024-126">Para que um usuário não administrador cancele sua própria solicitação, a solicitação deve conter a **id** do [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) e um **requestStatus** com um valor `cancelled` de .</span><span class="sxs-lookup"><span data-stu-id="15024-126">For a non-administrator user to cancel their own request, the request must contain the **id** of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) and a **requestStatus** with a value of `cancelled`.</span></span>

## <a name="response"></a><span data-ttu-id="15024-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="15024-127">Response</span></span>

<span data-ttu-id="15024-128">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="15024-128">If successful, this method returns a `200 OK` response code.</span></span>  <span data-ttu-id="15024-129">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15024-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15024-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="15024-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15024-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15024-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="15024-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="15024-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel

{
  "id":"request-id",
  "requestStatus":"cancelled"
}
```
# <a name="javascript"></a>[<span data-ttu-id="15024-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15024-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15024-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15024-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="15024-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="15024-135">Response</span></span>
<span data-ttu-id="15024-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="15024-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

