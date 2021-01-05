---
title: Atualizar accessPackageAssignmentPolicy
description: Atualiza as propriedades de um objeto accessPackageAssignmentPolicy.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 12819c9f79e243289ddbbfce380be1687694dc79
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752795"
---
# <a name="update-accesspackageassignmentpolicy"></a><span data-ttu-id="497fa-103">Atualizar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="497fa-103">Update accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="497fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="497fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497fa-105">Atualize um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) existente para alterar uma ou mais de suas propriedades, como o nome para exibição ou a descrição.</span><span class="sxs-lookup"><span data-stu-id="497fa-105">Update an existing [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="497fa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="497fa-106">Permissions</span></span>
<span data-ttu-id="497fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="497fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="497fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="497fa-109">Permission type</span></span>|<span data-ttu-id="497fa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="497fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="497fa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="497fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="497fa-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497fa-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="497fa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="497fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="497fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="497fa-114">Not supported.</span></span> |
|<span data-ttu-id="497fa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="497fa-115">Application</span></span>                            | <span data-ttu-id="497fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="497fa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="497fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="497fa-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```
## <a name="request-headers"></a><span data-ttu-id="497fa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="497fa-118">Request headers</span></span>
|<span data-ttu-id="497fa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="497fa-119">Name</span></span>|<span data-ttu-id="497fa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="497fa-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="497fa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="497fa-121">Authorization</span></span>|<span data-ttu-id="497fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="497fa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="497fa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="497fa-124">Content-Type</span></span>|<span data-ttu-id="497fa-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="497fa-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="497fa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="497fa-127">Request body</span></span>
<span data-ttu-id="497fa-128">No corpo da solicitação, forneça uma representação JSON do objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="497fa-128">In the request body, supply a JSON representation of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

<span data-ttu-id="497fa-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar um [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="497fa-129">The following table shows the properties that are required when you update an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

|<span data-ttu-id="497fa-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="497fa-130">Property</span></span>|<span data-ttu-id="497fa-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="497fa-131">Type</span></span>|<span data-ttu-id="497fa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="497fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="497fa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="497fa-133">displayName</span></span>|<span data-ttu-id="497fa-134">String</span><span class="sxs-lookup"><span data-stu-id="497fa-134">String</span></span>|<span data-ttu-id="497fa-135">O nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="497fa-135">The display name of the policy.</span></span>|
|<span data-ttu-id="497fa-136">description</span><span class="sxs-lookup"><span data-stu-id="497fa-136">description</span></span>|<span data-ttu-id="497fa-137">String</span><span class="sxs-lookup"><span data-stu-id="497fa-137">String</span></span>|<span data-ttu-id="497fa-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="497fa-138">The description of the policy.</span></span>|
|<span data-ttu-id="497fa-139">exextend</span><span class="sxs-lookup"><span data-stu-id="497fa-139">canExtend</span></span>|<span data-ttu-id="497fa-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="497fa-140">Boolean</span></span>|<span data-ttu-id="497fa-141">Indica se um usuário pode estender a duração da atribuição de pacote de acesso após a aprovação.</span><span class="sxs-lookup"><span data-stu-id="497fa-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="497fa-142">durationInDays</span><span class="sxs-lookup"><span data-stu-id="497fa-142">durationInDays</span></span>|<span data-ttu-id="497fa-143">Int32</span><span class="sxs-lookup"><span data-stu-id="497fa-143">Int32</span></span>|<span data-ttu-id="497fa-144">O número de dias em que as atribuições dessa política duram até que tenham expirado.</span><span class="sxs-lookup"><span data-stu-id="497fa-144">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="497fa-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="497fa-145">expirationDateTime</span></span>|<span data-ttu-id="497fa-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="497fa-146">DateTimeOffset</span></span>|<span data-ttu-id="497fa-147">A data de validade das atribuições criadas nesta política.</span><span class="sxs-lookup"><span data-stu-id="497fa-147">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="497fa-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="497fa-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="497fa-149">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="497fa-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="497fa-150">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="497fa-150">requestorSettings</span></span>|[<span data-ttu-id="497fa-151">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="497fa-151">requestorSettings</span></span>](../resources/requestorsettings.md)|<span data-ttu-id="497fa-152">Quem pode solicitar esse pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="497fa-152">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="497fa-153">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="497fa-153">requestApprovalSettings</span></span>|[<span data-ttu-id="497fa-154">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="497fa-154">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="497fa-155">Quem deve aprovar solicitações de pacote do Access nessa política.</span><span class="sxs-lookup"><span data-stu-id="497fa-155">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="497fa-156">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="497fa-156">accessReviewSettings</span></span>|[<span data-ttu-id="497fa-157">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="497fa-157">assignmentReviewSettings</span></span>](../resources/assignmentreviewsettings.md)|<span data-ttu-id="497fa-158">Quem deve revisar e com que frequência as atribuições para o pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="497fa-158">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="497fa-159">Essa propriedade será nula se as revisões não forem necessárias.</span><span class="sxs-lookup"><span data-stu-id="497fa-159">This property is null if reviews are not required.</span></span>|


## <a name="response"></a><span data-ttu-id="497fa-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="497fa-160">Response</span></span>
<span data-ttu-id="497fa-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="497fa-161">If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>



## <a name="examples"></a><span data-ttu-id="497fa-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="497fa-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="497fa-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="497fa-163">Request</span></span>
<span data-ttu-id="497fa-164">Nesta atualização de política, uma das opções para a pergunta de múltipla escolha foi removida.</span><span class="sxs-lookup"><span data-stu-id="497fa-164">In this policy update, one of the options for the multiple choice question was removed.</span></span> <span data-ttu-id="497fa-165">Os solicitantes futuros não terão mais a opção removida disponível.</span><span class="sxs-lookup"><span data-stu-id="497fa-165">Future requestors will no longer have the removed option available to them.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/b2eba9a1-b357-42ee-83a8-336522ed6cbf
Content-Type: application/json
Content-length: 1000

{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "4c02f928-7752-49aa-8fc8-e286d973a965",
    "displayName": "All Users",
    "description": "All users can request for access to the directory.",
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
        "approvalMode": "SingleStage",
        "approvalStages": [{
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
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
    "accessReviewSettings": {
        "isEnabled": false
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


# <a name="java"></a>[<span data-ttu-id="497fa-166">Java</span><span class="sxs-lookup"><span data-stu-id="497fa-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="497fa-167">C#</span><span class="sxs-lookup"><span data-stu-id="497fa-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="497fa-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="497fa-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="497fa-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="497fa-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="497fa-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="497fa-170">Response</span></span>
<span data-ttu-id="497fa-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="497fa-171">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "4c02f928-7752-49aa-8fc8-e286d973a965",
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

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


