---
title: Tipo de recurso accessPackageAssignmentPolicy
description: Uma política de atribuição de pacote de acesso especifica a política pela qual os titulares podem solicitar ou ser atribuídos um pacote de acesso por meio de uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: db463609803e3547b88f586cc447974846738e22
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720442"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="f103b-103">Tipo de recurso accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f103b-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="f103b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f103b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f103b-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma política de atribuição de pacote de acesso especifica a política pela qual os titulares podem solicitar ou ter um pacote de acesso atribuído por meio de uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="f103b-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="f103b-106">Um pacote de acesso pode ter zero ou mais políticas.</span><span class="sxs-lookup"><span data-stu-id="f103b-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="f103b-107">Quando uma solicitação de um assunto é recebida, o assunto é corresponder a cada política para encontrar a política (se alguma) com requestorSettings que incluem esse assunto.</span><span class="sxs-lookup"><span data-stu-id="f103b-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="f103b-108">Em seguida, a política determina se a solicitação requer aprovação, a duração da atribuição do pacote de acesso e se a atribuição precisa ser revisada regularmente.</span><span class="sxs-lookup"><span data-stu-id="f103b-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="f103b-109">Para atribuir um usuário a um pacote de acesso, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faz referência ao pacote de acesso e à política de atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="f103b-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="f103b-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="f103b-110">Methods</span></span>

| <span data-ttu-id="f103b-111">Método</span><span class="sxs-lookup"><span data-stu-id="f103b-111">Method</span></span>       | <span data-ttu-id="f103b-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f103b-112">Return Type</span></span> | <span data-ttu-id="f103b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f103b-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f103b-114">Listar accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="f103b-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="f103b-115">[coleção accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f103b-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="f103b-116">Recupere uma lista de objetos accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="f103b-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="f103b-117">Criar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f103b-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="f103b-118">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f103b-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="f103b-119">Crie um novo objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="f103b-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="f103b-120">Obter accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f103b-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="f103b-121">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f103b-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="f103b-122">Ler propriedades e relações de um objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="f103b-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="f103b-123">Atualizar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f103b-123">Update accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-update.md)|[<span data-ttu-id="f103b-124">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f103b-124">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="f103b-125">Atualize as propriedades de um objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="f103b-125">Update the properties of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="f103b-126">Excluir accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f103b-126">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="f103b-127">Exclua um accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="f103b-127">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="f103b-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f103b-128">Properties</span></span>

| <span data-ttu-id="f103b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f103b-129">Property</span></span>     | <span data-ttu-id="f103b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f103b-130">Type</span></span>        | <span data-ttu-id="f103b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f103b-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f103b-132">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="f103b-132">accessPackageId</span></span>|<span data-ttu-id="f103b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f103b-133">String</span></span>|<span data-ttu-id="f103b-134">ID do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="f103b-134">ID of the access package.</span></span>|
|<span data-ttu-id="f103b-135">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="f103b-135">accessReviewSettings</span></span>|[<span data-ttu-id="f103b-136">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="f103b-136">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="f103b-137">Quem deve revisar e com que frequência as atribuições para o pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="f103b-137">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="f103b-138">Essa propriedade será nula se as avaliações não são necessárias.</span><span class="sxs-lookup"><span data-stu-id="f103b-138">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="f103b-139">canExtend</span><span class="sxs-lookup"><span data-stu-id="f103b-139">canExtend</span></span>|<span data-ttu-id="f103b-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="f103b-140">Boolean</span></span>|<span data-ttu-id="f103b-141">Indica se um usuário pode estender a duração da atribuição do pacote de acesso após a aprovação.</span><span class="sxs-lookup"><span data-stu-id="f103b-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="f103b-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="f103b-142">createdBy</span></span>|<span data-ttu-id="f103b-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f103b-143">String</span></span>|<span data-ttu-id="f103b-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f103b-144">Read-only.</span></span>|
|<span data-ttu-id="f103b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f103b-145">createdDateTime</span></span>|<span data-ttu-id="f103b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f103b-146">DateTimeOffset</span></span>|<span data-ttu-id="f103b-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f103b-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f103b-148">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="f103b-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f103b-149">description</span><span class="sxs-lookup"><span data-stu-id="f103b-149">description</span></span>|<span data-ttu-id="f103b-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f103b-150">String</span></span>|<span data-ttu-id="f103b-151">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="f103b-151">The description of the policy.</span></span>|
|<span data-ttu-id="f103b-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f103b-152">displayName</span></span>|<span data-ttu-id="f103b-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f103b-153">String</span></span>|<span data-ttu-id="f103b-154">O nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="f103b-154">The display name of the policy.</span></span>|
|<span data-ttu-id="f103b-155">durationInDays</span><span class="sxs-lookup"><span data-stu-id="f103b-155">durationInDays</span></span>|<span data-ttu-id="f103b-156">Int32</span><span class="sxs-lookup"><span data-stu-id="f103b-156">Int32</span></span>|<span data-ttu-id="f103b-157">O número de dias em que as atribuições dessa política duram até expirar.</span><span class="sxs-lookup"><span data-stu-id="f103b-157">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="f103b-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f103b-158">expirationDateTime</span></span>|<span data-ttu-id="f103b-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f103b-159">DateTimeOffset</span></span>|<span data-ttu-id="f103b-160">A data de expiração das atribuições criadas nesta política.</span><span class="sxs-lookup"><span data-stu-id="f103b-160">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="f103b-161">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f103b-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f103b-162">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="f103b-162">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f103b-163">id</span><span class="sxs-lookup"><span data-stu-id="f103b-163">id</span></span>|<span data-ttu-id="f103b-164">String</span><span class="sxs-lookup"><span data-stu-id="f103b-164">String</span></span>| <span data-ttu-id="f103b-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f103b-165">Read-only.</span></span>|
|<span data-ttu-id="f103b-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="f103b-166">modifiedBy</span></span>|<span data-ttu-id="f103b-167">String</span><span class="sxs-lookup"><span data-stu-id="f103b-167">String</span></span>|<span data-ttu-id="f103b-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f103b-168">Read-only.</span></span>|
|<span data-ttu-id="f103b-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f103b-169">modifiedDateTime</span></span>|<span data-ttu-id="f103b-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f103b-170">DateTimeOffset</span></span>|<span data-ttu-id="f103b-171">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f103b-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f103b-172">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="f103b-172">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f103b-173">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="f103b-173">requestApprovalSettings</span></span>|[<span data-ttu-id="f103b-174">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="f103b-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="f103b-175">Quem deve aprovar solicitações de pacote de acesso nesta política.</span><span class="sxs-lookup"><span data-stu-id="f103b-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="f103b-176">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="f103b-176">requestorSettings</span></span>|[<span data-ttu-id="f103b-177">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="f103b-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="f103b-178">Quem pode solicitar esse pacote de acesso a partir dessa política.</span><span class="sxs-lookup"><span data-stu-id="f103b-178">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="f103b-179">questions</span><span class="sxs-lookup"><span data-stu-id="f103b-179">questions</span></span>|<span data-ttu-id="f103b-180">[Coleção accessPackageQuestion](accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="f103b-180">[accessPackageQuestion](accesspackagequestion.md) collection</span></span>|<span data-ttu-id="f103b-181">Perguntas que são colocadas ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="f103b-181">Questions that are posed to the  requestor.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f103b-182">Relações</span><span class="sxs-lookup"><span data-stu-id="f103b-182">Relationships</span></span>

| <span data-ttu-id="f103b-183">Relação</span><span class="sxs-lookup"><span data-stu-id="f103b-183">Relationship</span></span> | <span data-ttu-id="f103b-184">Tipo</span><span class="sxs-lookup"><span data-stu-id="f103b-184">Type</span></span>        | <span data-ttu-id="f103b-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="f103b-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f103b-186">accessPackage</span><span class="sxs-lookup"><span data-stu-id="f103b-186">accessPackage</span></span>|[<span data-ttu-id="f103b-187">accessPackage</span><span class="sxs-lookup"><span data-stu-id="f103b-187">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="f103b-188">O pacote de acesso com essa política.</span><span class="sxs-lookup"><span data-stu-id="f103b-188">The access package with this policy.</span></span> <span data-ttu-id="f103b-189">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f103b-189">Read-only.</span></span> <span data-ttu-id="f103b-190">Anulável.</span><span class="sxs-lookup"><span data-stu-id="f103b-190">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f103b-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f103b-191">JSON representation</span></span>

<span data-ttu-id="f103b-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f103b-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "keyProperty": "id"
}-->

```json
{
    "id": "string",
    "accessPackageId": "string",
    "displayName": "string",
    "description": "string",
    "isDenyPolicy": false,
    "canExtend": false,
    "durationInDays": 365,
    "requestorSettings": {
        "scopeType": "string",
        "acceptRequests": true,
        "allowedRequestors": [{
            "@odata.type": "#microsoft.graph.userSet"
        }]
    },
    "requestApprovalSettings": {
        "isApprovalRequired": false,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": false,
        "approvalMode": "string",
        "approvalStages": [{
            "approvalStageTimeOutInDays": 14,
            "isApproverJustificationRequired": true,
            "isEscalationEnabled": true,
            "escalationTimeInMinutes": 11520,
            "primaryApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }],
            "escalationApprovers": [{
                "@odata.type": "#microsoft.graph.userSet"
            }]
        }]
    },
    "accessReviewSettings": null,
    "questions": [{
        "@odata.type": "#microsoft.graph.question"
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

