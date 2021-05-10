---
title: 'accessPackageAssignmentRequest: cancel'
description: Cancele os objetos accessPackageAssignmentRequest que estão em estado cancelável.
localization_priority: Normal
author: sbounouh
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5079de33f7ef3c7536baf50a876a84d5ca3711b4
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299014"
---
# <a name="accesspackageassignmentrequest-cancel"></a><span data-ttu-id="35df0-103">accessPackageAssignmentRequest: cancel</span><span class="sxs-lookup"><span data-stu-id="35df0-103">accessPackageAssignmentRequest: cancel</span></span>
<span data-ttu-id="35df0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35df0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35df0-105">No [Azure AD Entitlement Management,](../resources/entitlementmanagement-root.md)cancele os objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) que estão em estado cancelável: `accepted` , , , `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated` .</span><span class="sxs-lookup"><span data-stu-id="35df0-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), cancel [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects that are in a cancellable state: `accepted`, `pendingApproval`, `pendingNotBefore`, `pendingApprovalEscalated`.</span></span>

## <a name="permissions"></a><span data-ttu-id="35df0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35df0-106">Permissions</span></span>
<span data-ttu-id="35df0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35df0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35df0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35df0-109">Permission type</span></span>|<span data-ttu-id="35df0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35df0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35df0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35df0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35df0-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35df0-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="35df0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35df0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35df0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35df0-114">Not supported.</span></span>|
|<span data-ttu-id="35df0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35df0-115">Application</span></span>|<span data-ttu-id="35df0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35df0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35df0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35df0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="35df0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35df0-118">Request headers</span></span>
|<span data-ttu-id="35df0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="35df0-119">Name</span></span>|<span data-ttu-id="35df0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="35df0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="35df0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="35df0-121">Authorization</span></span>|<span data-ttu-id="35df0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35df0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35df0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35df0-124">Request body</span></span>
<span data-ttu-id="35df0-125">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="35df0-125">In the request body, supply a JSON representation of an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="35df0-126">Para que um usuário não administrador cancele sua própria solicitação, a solicitação deve conter a **id** do [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) e um **requestStatus** com um valor `cancelled` de .</span><span class="sxs-lookup"><span data-stu-id="35df0-126">For a non-administrator user to cancel their own request, the request must contain the **id** of the [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) and a **requestStatus** with a value of `cancelled`.</span></span>

## <a name="response"></a><span data-ttu-id="35df0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="35df0-127">Response</span></span>

<span data-ttu-id="35df0-128">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="35df0-128">If successful, this method returns a `200 OK` response code.</span></span>  <span data-ttu-id="35df0-129">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35df0-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35df0-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="35df0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35df0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35df0-131">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="35df0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="35df0-132">Response</span></span>
<span data-ttu-id="35df0-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35df0-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

