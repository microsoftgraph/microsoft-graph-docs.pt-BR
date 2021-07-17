---
title: Criar accessPackageAssignmentPolicy
description: Use essa API para criar um novo accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 707d3e7a11983f2ecc1ec9df9703582b01f33e2b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466954"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="657de-103">Criar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="657de-103">Create accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="657de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="657de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="657de-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)crie um novo [objeto accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="657de-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="657de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="657de-106">Permissions</span></span>

<span data-ttu-id="657de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="657de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="657de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="657de-109">Permission type</span></span>                        | <span data-ttu-id="657de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="657de-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="657de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="657de-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="657de-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="657de-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="657de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="657de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="657de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="657de-114">Not supported.</span></span> |
| <span data-ttu-id="657de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="657de-115">Application</span></span>                            | <span data-ttu-id="657de-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="657de-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="657de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="657de-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="657de-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="657de-118">Request headers</span></span>

| <span data-ttu-id="657de-119">Nome</span><span class="sxs-lookup"><span data-stu-id="657de-119">Name</span></span>          | <span data-ttu-id="657de-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="657de-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="657de-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="657de-121">Authorization</span></span> | <span data-ttu-id="657de-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="657de-p102">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="657de-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="657de-124">Content-Type</span></span>  | <span data-ttu-id="657de-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="657de-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="657de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="657de-127">Request body</span></span>

<span data-ttu-id="657de-128">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="657de-128">In the request body, supply a JSON representation of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="657de-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="657de-129">Response</span></span>

<span data-ttu-id="657de-130">Se tiver êxito, este método retornará um código de resposta de 200 séries e um novo [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="657de-130">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="657de-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="657de-131">Examples</span></span>

### <a name="example-1-create-a-direct-assignment-policy"></a><span data-ttu-id="657de-132">Exemplo 1: Criar uma política de atribuição direta</span><span class="sxs-lookup"><span data-stu-id="657de-132">Example 1: Create a direct assignment policy</span></span>

<span data-ttu-id="657de-133">Uma política de atribuição direta é útil quando as solicitações de atribuição de pacote de acesso só serão criadas por um administrador, não pelos próprios usuários.</span><span class="sxs-lookup"><span data-stu-id="657de-133">A direct assignment policy is useful when access package assignment requests will only be created by an administrator, not by users themselves.</span></span>

#### <a name="request"></a><span data-ttu-id="657de-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="657de-134">Request</span></span>

<span data-ttu-id="657de-135">O exemplo a seguir mostra uma solicitação para criar uma política de atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="657de-135">The following example shows a request to create an access package assignment policy.</span></span> <span data-ttu-id="657de-136">Nesta política, nenhum usuário pode solicitar, nenhuma aprovação é necessária e não há críticas de acesso.</span><span class="sxs-lookup"><span data-stu-id="657de-136">In this policy, no users can request, no approval is required, and there are no access reviews.</span></span>

# <a name="http"></a>[<span data-ttu-id="657de-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="657de-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="657de-138">C#</span><span class="sxs-lookup"><span data-stu-id="657de-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="657de-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="657de-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="657de-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="657de-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="657de-141">Java</span><span class="sxs-lookup"><span data-stu-id="657de-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="657de-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="657de-142">Response</span></span>

<span data-ttu-id="657de-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="657de-143">The following is an example of the response.</span></span>

> <span data-ttu-id="657de-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="657de-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-policy-for-users-from-other-organizations-to-request"></a><span data-ttu-id="657de-145">Exemplo 2: criar uma política para usuários de outras organizações solicitarem</span><span class="sxs-lookup"><span data-stu-id="657de-145">Example 2: Create a policy for users from other organizations to request</span></span>

<span data-ttu-id="657de-146">O exemplo a seguir mostra uma política mais complexa com aprovações de dois estágios e avaliações de acesso.</span><span class="sxs-lookup"><span data-stu-id="657de-146">The following example shows a more complex policy with two-stage approvals and access reviews.</span></span>

#### <a name="request"></a><span data-ttu-id="657de-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="657de-147">Request</span></span>

<span data-ttu-id="657de-148">A seguir, um exemplo da solicitação para criar uma política de atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="657de-148">The following is an example of the request to create an access package assignment policy.</span></span> 


# <a name="http"></a>[<span data-ttu-id="657de-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="657de-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="657de-150">C#</span><span class="sxs-lookup"><span data-stu-id="657de-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="657de-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="657de-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="657de-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="657de-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="657de-153">Java</span><span class="sxs-lookup"><span data-stu-id="657de-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="657de-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="657de-154">Response</span></span>

<span data-ttu-id="657de-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="657de-155">The following is an example of the response.</span></span>

> <span data-ttu-id="657de-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="657de-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-assignment-policy-with-questions"></a><span data-ttu-id="657de-157">Exemplo 3: Criar política de atribuição com perguntas</span><span class="sxs-lookup"><span data-stu-id="657de-157">Example 3: Create assignment policy with questions</span></span>

<span data-ttu-id="657de-158">Perguntas configuradas em uma política de atribuição serão feitas aos solicitadores no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="657de-158">Questions configured in an assignment policy will be asked to requestors in scope of the policy.</span></span> <span data-ttu-id="657de-159">Suas respostas serão mostradas aos aprovadores.</span><span class="sxs-lookup"><span data-stu-id="657de-159">Their answers will be shown to their approvers.</span></span> <span data-ttu-id="657de-160">As IDs de perguntas são somente leitura e são incluídas na resposta por padrão.</span><span class="sxs-lookup"><span data-stu-id="657de-160">Question IDs are read-only and are included in the response by default.</span></span>

#### <a name="request"></a><span data-ttu-id="657de-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="657de-161">Request</span></span>

<span data-ttu-id="657de-162">O exemplo a seguir mostra uma solicitação para criar uma política de atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="657de-162">The following example shows a request to create an access package assignment policy.</span></span> 



# <a name="http"></a>[<span data-ttu-id="657de-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="657de-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies_questions"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
    "accessPackageId": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "displayName": "Users from connected organizations can request",
    "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
    "canExtend": false,
    "durationInDays": 365,
    "expirationDateTime": null,
    "requestorSettings": {
        "scopeType": "AllExistingConnectedOrganizationSubjects",
        "acceptRequests": true
    },
    "requestApprovalSettings": {
        "isApprovalRequired": true,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": true,
        "approvalMode": "SingleStage",
        "approvalStages": [{
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": false,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [{
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "d2dcb9a1-a445-42ee-83a8-476522ed6cbf",
                        "description": "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.externalSponsors",
                        "isBackup": false
                    }
                ]
            }
        ]
    },
    "questions": [{
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "OH",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Ohio",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
}
```
# <a name="c"></a>[<span data-ttu-id="657de-164">C#</span><span class="sxs-lookup"><span data-stu-id="657de-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="657de-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="657de-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="657de-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="657de-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="657de-167">Java</span><span class="sxs-lookup"><span data-stu-id="657de-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---

#### <a name="response"></a><span data-ttu-id="657de-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="657de-168">Response</span></span>

<span data-ttu-id="657de-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="657de-169">The following is an example of the response.</span></span>

> <span data-ttu-id="657de-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="657de-170">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
  "questions": [{
        "id" : "BD3F6B95-458D-4BC8-A9A6-8D4B29F64F3D",
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona?",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "OH",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Ohio",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "id" : "F652C13C-A660-4E4C-A1E0-CE9FEC6EE57A",
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
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


