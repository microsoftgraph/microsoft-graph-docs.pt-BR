---
title: Atualizar accessPackageAssignmentPolicy
description: Atualizar as propriedades de um objeto accessPackageAssignmentPolicy.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2a82476a61fbc775e894f5c5baf0444468041ab5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872111"
---
# <a name="update-accesspackageassignmentpolicy"></a><span data-ttu-id="7e687-103">Atualizar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="7e687-103">Update accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="7e687-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e687-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e687-105">Atualize um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) existente para alterar uma ou mais de suas propriedades, como o nome de exibição ou a descrição.</span><span class="sxs-lookup"><span data-stu-id="7e687-105">Update an existing [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e687-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e687-106">Permissions</span></span>
<span data-ttu-id="7e687-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e687-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="7e687-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e687-109">Permission type</span></span>|<span data-ttu-id="7e687-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e687-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e687-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e687-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e687-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e687-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="7e687-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e687-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e687-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e687-114">Not supported.</span></span> |
|<span data-ttu-id="7e687-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e687-115">Application</span></span>                            | <span data-ttu-id="7e687-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e687-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e687-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e687-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```
## <a name="request-headers"></a><span data-ttu-id="7e687-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e687-118">Request headers</span></span>
|<span data-ttu-id="7e687-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7e687-119">Name</span></span>|<span data-ttu-id="7e687-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e687-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7e687-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e687-121">Authorization</span></span>|<span data-ttu-id="7e687-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e687-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7e687-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e687-124">Content-Type</span></span>|<span data-ttu-id="7e687-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e687-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e687-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e687-127">Request body</span></span>
<span data-ttu-id="7e687-128">No corpo da solicitação, fornece uma representação JSON do [objeto accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7e687-128">In the request body, supply a JSON representation of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

<span data-ttu-id="7e687-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [um accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7e687-129">The following table shows the properties that are required when you update an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

|<span data-ttu-id="7e687-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e687-130">Property</span></span>|<span data-ttu-id="7e687-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e687-131">Type</span></span>|<span data-ttu-id="7e687-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e687-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e687-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7e687-133">displayName</span></span>|<span data-ttu-id="7e687-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e687-134">String</span></span>|<span data-ttu-id="7e687-135">O nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="7e687-135">The display name of the policy.</span></span>|
|<span data-ttu-id="7e687-136">description</span><span class="sxs-lookup"><span data-stu-id="7e687-136">description</span></span>|<span data-ttu-id="7e687-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e687-137">String</span></span>|<span data-ttu-id="7e687-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="7e687-138">The description of the policy.</span></span>|
|<span data-ttu-id="7e687-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="7e687-139">canExtend</span></span>|<span data-ttu-id="7e687-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e687-140">Boolean</span></span>|<span data-ttu-id="7e687-141">Indica se um usuário pode estender a duração da atribuição do pacote de acesso após a aprovação.</span><span class="sxs-lookup"><span data-stu-id="7e687-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="7e687-142">durationInDays</span><span class="sxs-lookup"><span data-stu-id="7e687-142">durationInDays</span></span>|<span data-ttu-id="7e687-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7e687-143">Int32</span></span>|<span data-ttu-id="7e687-144">O número de dias em que as atribuições dessa política duram até expirar.</span><span class="sxs-lookup"><span data-stu-id="7e687-144">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="7e687-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7e687-145">expirationDateTime</span></span>|<span data-ttu-id="7e687-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e687-146">DateTimeOffset</span></span>|<span data-ttu-id="7e687-147">A data de expiração das atribuições criadas nesta política.</span><span class="sxs-lookup"><span data-stu-id="7e687-147">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="7e687-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7e687-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7e687-149">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7e687-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7e687-150">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="7e687-150">requestorSettings</span></span>|[<span data-ttu-id="7e687-151">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="7e687-151">requestorSettings</span></span>](../resources/requestorsettings.md)|<span data-ttu-id="7e687-152">Quem pode solicitar esse pacote de acesso a partir dessa política.</span><span class="sxs-lookup"><span data-stu-id="7e687-152">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="7e687-153">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="7e687-153">requestApprovalSettings</span></span>|[<span data-ttu-id="7e687-154">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="7e687-154">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="7e687-155">Quem deve aprovar solicitações para o pacote de acesso nesta política.</span><span class="sxs-lookup"><span data-stu-id="7e687-155">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="7e687-156">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="7e687-156">accessReviewSettings</span></span>|[<span data-ttu-id="7e687-157">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="7e687-157">assignmentReviewSettings</span></span>](../resources/assignmentreviewsettings.md)|<span data-ttu-id="7e687-158">Quem deve revisar e com que frequência as atribuições para o pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="7e687-158">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="7e687-159">Essa propriedade será nula se as análises não são necessárias.</span><span class="sxs-lookup"><span data-stu-id="7e687-159">This property is null if reviews are not required.</span></span>|


## <a name="response"></a><span data-ttu-id="7e687-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e687-160">Response</span></span>
<span data-ttu-id="7e687-161">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e687-161">If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>



## <a name="examples"></a><span data-ttu-id="7e687-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7e687-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e687-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e687-163">Request</span></span>
<span data-ttu-id="7e687-164">Nesta atualização de política, uma das opções para a pergunta de múltipla escolha foi removida.</span><span class="sxs-lookup"><span data-stu-id="7e687-164">In this policy update, one of the options for the multiple choice question was removed.</span></span> <span data-ttu-id="7e687-165">Os futuros solicitadores não terão mais a opção removida disponível para eles.</span><span class="sxs-lookup"><span data-stu-id="7e687-165">Future requestors will no longer have the removed option available to them.</span></span>

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


# <a name="java"></a>[<span data-ttu-id="7e687-166">Java</span><span class="sxs-lookup"><span data-stu-id="7e687-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7e687-167">C#</span><span class="sxs-lookup"><span data-stu-id="7e687-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e687-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e687-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e687-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e687-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7e687-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e687-170">Response</span></span>
<span data-ttu-id="7e687-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7e687-171">**Note:** The response object shown here might be shortened for readability.</span></span>
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


