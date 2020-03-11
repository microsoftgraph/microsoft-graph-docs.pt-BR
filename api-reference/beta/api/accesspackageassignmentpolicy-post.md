---
title: Criar accessPackageAssignmentPolicy
description: Use esta API para criar um novo accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d49306eec7e7643fe5f380950667f319c433523
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589703"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="e0116-103">Criar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="e0116-103">Create accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="e0116-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0116-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0116-105">Em [Gerenciamento de qualificação do Azure ad](../resources/entitlementmanagement-root.md), crie um novo objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e0116-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0116-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0116-106">Permissions</span></span>

<span data-ttu-id="e0116-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0116-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0116-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0116-109">Permission type</span></span>                        | <span data-ttu-id="e0116-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0116-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e0116-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0116-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0116-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0116-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="e0116-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0116-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0116-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0116-114">Not supported.</span></span> |
| <span data-ttu-id="e0116-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0116-115">Application</span></span>                            | <span data-ttu-id="e0116-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0116-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0116-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0116-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e0116-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0116-118">Request headers</span></span>

| <span data-ttu-id="e0116-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e0116-119">Name</span></span>          | <span data-ttu-id="e0116-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0116-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e0116-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0116-121">Authorization</span></span> | <span data-ttu-id="e0116-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="e0116-122">Bearer \{token\}.</span></span> <span data-ttu-id="e0116-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0116-123">Required.</span></span> |
| <span data-ttu-id="e0116-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0116-124">Content-Type</span></span>  | <span data-ttu-id="e0116-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0116-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0116-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0116-127">Request body</span></span>

<span data-ttu-id="e0116-128">No corpo da solicitação, forneça uma representação JSON de um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e0116-128">In the request body, supply a JSON representation of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0116-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0116-129">Response</span></span>

<span data-ttu-id="e0116-130">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0116-130">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0116-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e0116-131">Examples</span></span>

### <a name="example-1-create-a-direct-assignment-policy"></a><span data-ttu-id="e0116-132">Exemplo 1: criar uma política de atribuição direta</span><span class="sxs-lookup"><span data-stu-id="e0116-132">Example 1: Create a direct assignment policy</span></span>

<span data-ttu-id="e0116-133">Uma política de atribuição direta é útil quando as solicitações de atribuição de pacote de acesso só serão criadas por um administrador, e não pelos próprios usuários.</span><span class="sxs-lookup"><span data-stu-id="e0116-133">A direct assignment policy is useful when access package assignment requests will only be created by an administrator, not by users themselves.</span></span>

#### <a name="request"></a><span data-ttu-id="e0116-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0116-134">Request</span></span>

<span data-ttu-id="e0116-135">O exemplo a seguir mostra uma solicitação para criar uma política de atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="e0116-135">The following example shows a request to create an access package assignment policy.</span></span> <span data-ttu-id="e0116-136">Nesta política, nenhum usuário pode solicitar, nenhuma aprovação é necessária e não há nenhuma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="e0116-136">In this policy, no users can request, no approval is required, and there are no access reviews.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0116-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0116-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "NoSubjects",
    "acceptRequests": true,
    "allowedRequestors": []
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```
# <a name="c"></a>[<span data-ttu-id="e0116-138">C#</span><span class="sxs-lookup"><span data-stu-id="e0116-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0116-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0116-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0116-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0116-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e0116-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0116-141">Response</span></span>

<span data-ttu-id="e0116-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0116-142">The following is an example of the response.</span></span>

> <span data-ttu-id="e0116-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0116-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator"
}
```

### <a name="example-2-create-a-policy-for-users-from-other-organizations-to-request"></a><span data-ttu-id="e0116-145">Exemplo 2: criar uma política para usuários de outras organizações solicitarem</span><span class="sxs-lookup"><span data-stu-id="e0116-145">Example 2: Create a policy for users from other organizations to request</span></span>

<span data-ttu-id="e0116-146">O exemplo a seguir mostra uma política mais complexa com aprovações de dois estágios e revisões de acesso.</span><span class="sxs-lookup"><span data-stu-id="e0116-146">The following example shows a more complex policy with two-stage approvals and access reviews.</span></span>

#### <a name="request"></a><span data-ttu-id="e0116-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0116-147">Request</span></span>

<span data-ttu-id="e0116-148">Veja a seguir um exemplo de solicitação para criar uma política de atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="e0116-148">The following is an example of the request to create an access package assignment policy.</span></span> 


# <a name="http"></a>[<span data-ttu-id="e0116-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0116-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies_multistage"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
    "accessPackageId": "string (identifier)",
    "displayName": "Users from connected organizations can request",
    "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
    "canExtend": false,
    "durationInDays": 365,
    "expirationDateTime": null,
    "requestorSettings": {
        "scopeType": "AllExistingConnectedOrganizationSubjects",
        "acceptRequests": true,
        "allowedRequestors": []
    },
    "requestApprovalSettings": {
        "isApprovalRequired": true,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": true,
        "approvalMode": "Serial",
        "approvalStages": [
            {
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.externalSponsors",
                        "isBackup": false
                    }
                ],
                "escalationApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.singleUser",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "user if the external sponsor does not respond"
                    }
                ]
            },
            {
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "group for users from connected organizations which have no internal sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.internalSponsors",
                        "isBackup": false
                    }
                ],
                "escalationApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.singleUser",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "user if the internal sponsor does not respond"
                    }
                ]
            }
        ]
    },
    "accessReviewSettings": {
        "isEnabled": true,
        "recurrenceType": "quarterly",
        "reviewerType": "Self",
        "startDateTime": "2020-04-01T07:59:59.998Z",
        "durationInDays": 25,
        "reviewers": []
    }
}
```
# <a name="c"></a>[<span data-ttu-id="e0116-150">C#</span><span class="sxs-lookup"><span data-stu-id="e0116-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0116-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0116-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0116-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0116-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="e0116-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0116-153">Response</span></span>

<span data-ttu-id="e0116-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0116-154">The following is an example of the response.</span></span>

> <span data-ttu-id="e0116-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0116-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "string (identifier)",
  "displayName": "Users from connected organizations can request",
  "description": "Allow users from configured connected organizations to request and be approved by their sponsors"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
