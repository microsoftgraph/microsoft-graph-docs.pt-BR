---
title: Atualizar accessPackageAssignmentPolicy
description: Atualiza as propriedades de um objeto accessPackageAssignmentPolicy.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 086bc79bf6462d569f85e4abf885a8c8538356ae
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806391"
---
# <a name="update-accesspackageassignmentpolicy"></a><span data-ttu-id="391a2-103">Atualizar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="391a2-103">Update accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="391a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="391a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="391a2-105">Atualize um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) existente para alterar uma ou mais de suas propriedades, como o nome para exibição ou a descrição.</span><span class="sxs-lookup"><span data-stu-id="391a2-105">Update an existing [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="391a2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="391a2-106">Permissions</span></span>
<span data-ttu-id="391a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="391a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="391a2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="391a2-109">Permission type</span></span>|<span data-ttu-id="391a2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="391a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="391a2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="391a2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="391a2-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="391a2-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="391a2-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="391a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="391a2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="391a2-114">Not supported.</span></span> |
|<span data-ttu-id="391a2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="391a2-115">Application</span></span>                            | <span data-ttu-id="391a2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="391a2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="391a2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="391a2-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```
## <a name="request-headers"></a><span data-ttu-id="391a2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="391a2-118">Request headers</span></span>
|<span data-ttu-id="391a2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="391a2-119">Name</span></span>|<span data-ttu-id="391a2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="391a2-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="391a2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="391a2-121">Authorization</span></span>|<span data-ttu-id="391a2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="391a2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="391a2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="391a2-124">Content-Type</span></span>|<span data-ttu-id="391a2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="391a2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="391a2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="391a2-127">Request body</span></span>
<span data-ttu-id="391a2-128">No corpo da solicitação, forneça uma representação JSON do objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="391a2-128">In the request body, supply a JSON representation of the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

<span data-ttu-id="391a2-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar um [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="391a2-129">The following table shows the properties that are required when you update an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span>

|<span data-ttu-id="391a2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="391a2-130">Property</span></span>|<span data-ttu-id="391a2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="391a2-131">Type</span></span>|<span data-ttu-id="391a2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="391a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="391a2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="391a2-133">displayName</span></span>|<span data-ttu-id="391a2-134">String</span><span class="sxs-lookup"><span data-stu-id="391a2-134">String</span></span>|<span data-ttu-id="391a2-135">O nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="391a2-135">The display name of the policy.</span></span>|
|<span data-ttu-id="391a2-136">description</span><span class="sxs-lookup"><span data-stu-id="391a2-136">description</span></span>|<span data-ttu-id="391a2-137">String</span><span class="sxs-lookup"><span data-stu-id="391a2-137">String</span></span>|<span data-ttu-id="391a2-138">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="391a2-138">The description of the policy.</span></span>|
|<span data-ttu-id="391a2-139">exextend</span><span class="sxs-lookup"><span data-stu-id="391a2-139">canExtend</span></span>|<span data-ttu-id="391a2-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="391a2-140">Boolean</span></span>|<span data-ttu-id="391a2-141">Indica se um usuário pode estender a duração da atribuição de pacote de acesso após a aprovação.</span><span class="sxs-lookup"><span data-stu-id="391a2-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="391a2-142">durationInDays</span><span class="sxs-lookup"><span data-stu-id="391a2-142">durationInDays</span></span>|<span data-ttu-id="391a2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="391a2-143">Int32</span></span>|<span data-ttu-id="391a2-144">O número de dias em que as atribuições dessa política duram até que tenham expirado.</span><span class="sxs-lookup"><span data-stu-id="391a2-144">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="391a2-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="391a2-145">expirationDateTime</span></span>|<span data-ttu-id="391a2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="391a2-146">DateTimeOffset</span></span>|<span data-ttu-id="391a2-147">A data de validade das atribuições criadas nesta política.</span><span class="sxs-lookup"><span data-stu-id="391a2-147">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="391a2-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="391a2-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="391a2-149">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="391a2-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="391a2-150">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="391a2-150">requestorSettings</span></span>|[<span data-ttu-id="391a2-151">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="391a2-151">requestorSettings</span></span>](../resources/requestorsettings.md)|<span data-ttu-id="391a2-152">Quem pode solicitar esse pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="391a2-152">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="391a2-153">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="391a2-153">requestApprovalSettings</span></span>|[<span data-ttu-id="391a2-154">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="391a2-154">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="391a2-155">Quem deve aprovar solicitações de pacote do Access nessa política.</span><span class="sxs-lookup"><span data-stu-id="391a2-155">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="391a2-156">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="391a2-156">accessReviewSettings</span></span>|[<span data-ttu-id="391a2-157">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="391a2-157">assignmentReviewSettings</span></span>](../resources/assignmentreviewsettings.md)|<span data-ttu-id="391a2-158">Quem deve revisar e com que frequência as atribuições para o pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="391a2-158">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="391a2-159">Essa propriedade será nula se as revisões não forem necessárias.</span><span class="sxs-lookup"><span data-stu-id="391a2-159">This property is null if reviews are not required.</span></span>|


## <a name="response"></a><span data-ttu-id="391a2-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="391a2-160">Response</span></span>
<span data-ttu-id="391a2-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="391a2-161">If successful, this method returns a `200 OK` response code and an updated [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>



## <a name="examples"></a><span data-ttu-id="391a2-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="391a2-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="391a2-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="391a2-163">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="391a2-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="391a2-164">HTTP</span></span>](#tab/http)
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
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
  "canExtend": false,
  "durationInDays": 365,
  "requestorSettings" : {
    "scopeType": "AllExistingDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": []
  },
  "requestApprovalSettings" : {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  },
  "accessReviewSettings" : null
}
```
# <a name="javascript"></a>[<span data-ttu-id="391a2-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="391a2-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="391a2-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="391a2-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="391a2-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="391a2-167">Response</span></span>
<span data-ttu-id="391a2-168">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="391a2-168">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
  "canExtend": false,
  "durationInDays": 365,
  "accessReviewSettings" : null
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
