---
title: tipo de recurso accessPackageAssignmentPolicy
description: Uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c963030980e96c5baabe8bcfe9103d4dc5167979
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719759"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="229cb-103">tipo de recurso accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="229cb-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="229cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="229cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="229cb-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="229cb-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="229cb-106">Um pacote de acesso pode ter zero ou mais políticas.</span><span class="sxs-lookup"><span data-stu-id="229cb-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="229cb-107">Quando uma solicitação de um assunto é recebida, o assunto é correspondido em relação a cada política para localizar a política (se houver) com requestorSettings que inclua esse assunto.</span><span class="sxs-lookup"><span data-stu-id="229cb-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="229cb-108">A política determina se a solicitação requer aprovação, a duração da atribuição do pacote de acesso e se a atribuição precisa ser revisada regularmente.</span><span class="sxs-lookup"><span data-stu-id="229cb-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="229cb-109">Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="229cb-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="229cb-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="229cb-110">Methods</span></span>

| <span data-ttu-id="229cb-111">Método</span><span class="sxs-lookup"><span data-stu-id="229cb-111">Method</span></span>       | <span data-ttu-id="229cb-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="229cb-112">Return Type</span></span> | <span data-ttu-id="229cb-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="229cb-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="229cb-114">Listar accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="229cb-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="229cb-115">coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="229cb-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="229cb-116">Recupere uma lista de objetos accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="229cb-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="229cb-117">Criar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="229cb-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="229cb-118">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="229cb-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="229cb-119">Criar um novo objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="229cb-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="229cb-120">Obter accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="229cb-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="229cb-121">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="229cb-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="229cb-122">Ler propriedades e relações de um objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="229cb-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="229cb-123">Atualizar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="229cb-123">Update accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-update.md)|[<span data-ttu-id="229cb-124">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="229cb-124">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="229cb-125">Atualiza as propriedades de um objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="229cb-125">Update the properties of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="229cb-126">Excluir accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="229cb-126">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="229cb-127">Excluir um accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="229cb-127">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="229cb-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="229cb-128">Properties</span></span>

| <span data-ttu-id="229cb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="229cb-129">Property</span></span>     | <span data-ttu-id="229cb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="229cb-130">Type</span></span>        | <span data-ttu-id="229cb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="229cb-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="229cb-132">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="229cb-132">accessPackageId</span></span>|<span data-ttu-id="229cb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="229cb-133">String</span></span>|<span data-ttu-id="229cb-134">ID do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="229cb-134">ID of the access package.</span></span>|
|<span data-ttu-id="229cb-135">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="229cb-135">accessReviewSettings</span></span>|[<span data-ttu-id="229cb-136">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="229cb-136">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="229cb-137">Quem deve revisar e com que frequência as atribuições para o pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="229cb-137">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="229cb-138">Essa propriedade será nula se as revisões não forem necessárias.</span><span class="sxs-lookup"><span data-stu-id="229cb-138">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="229cb-139">exextend</span><span class="sxs-lookup"><span data-stu-id="229cb-139">canExtend</span></span>|<span data-ttu-id="229cb-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="229cb-140">Boolean</span></span>|<span data-ttu-id="229cb-141">Indica se um usuário pode estender a duração da atribuição de pacote de acesso após a aprovação.</span><span class="sxs-lookup"><span data-stu-id="229cb-141">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="229cb-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="229cb-142">createdBy</span></span>|<span data-ttu-id="229cb-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="229cb-143">String</span></span>|<span data-ttu-id="229cb-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="229cb-144">Read-only.</span></span>|
|<span data-ttu-id="229cb-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="229cb-145">createdDateTime</span></span>|<span data-ttu-id="229cb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="229cb-146">DateTimeOffset</span></span>|<span data-ttu-id="229cb-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="229cb-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="229cb-149">description</span><span class="sxs-lookup"><span data-stu-id="229cb-149">description</span></span>|<span data-ttu-id="229cb-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="229cb-150">String</span></span>|<span data-ttu-id="229cb-151">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="229cb-151">The description of the policy.</span></span>|
|<span data-ttu-id="229cb-152">displayName</span><span class="sxs-lookup"><span data-stu-id="229cb-152">displayName</span></span>|<span data-ttu-id="229cb-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="229cb-153">String</span></span>|<span data-ttu-id="229cb-154">O nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="229cb-154">The display name of the policy.</span></span>|
|<span data-ttu-id="229cb-155">durationInDays</span><span class="sxs-lookup"><span data-stu-id="229cb-155">durationInDays</span></span>|<span data-ttu-id="229cb-156">Int32</span><span class="sxs-lookup"><span data-stu-id="229cb-156">Int32</span></span>|<span data-ttu-id="229cb-157">O número de dias em que as atribuições dessa política duram até que tenham expirado.</span><span class="sxs-lookup"><span data-stu-id="229cb-157">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="229cb-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="229cb-158">expirationDateTime</span></span>|<span data-ttu-id="229cb-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="229cb-159">DateTimeOffset</span></span>|<span data-ttu-id="229cb-160">A data de validade das atribuições criadas nesta política.</span><span class="sxs-lookup"><span data-stu-id="229cb-160">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="229cb-161">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="229cb-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="229cb-162">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="229cb-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="229cb-163">id</span><span class="sxs-lookup"><span data-stu-id="229cb-163">id</span></span>|<span data-ttu-id="229cb-164">String</span><span class="sxs-lookup"><span data-stu-id="229cb-164">String</span></span>| <span data-ttu-id="229cb-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="229cb-165">Read-only.</span></span>|
|<span data-ttu-id="229cb-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="229cb-166">modifiedBy</span></span>|<span data-ttu-id="229cb-167">String</span><span class="sxs-lookup"><span data-stu-id="229cb-167">String</span></span>|<span data-ttu-id="229cb-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="229cb-168">Read-only.</span></span>|
|<span data-ttu-id="229cb-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="229cb-169">modifiedDateTime</span></span>|<span data-ttu-id="229cb-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="229cb-170">DateTimeOffset</span></span>|<span data-ttu-id="229cb-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="229cb-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="229cb-173">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="229cb-173">requestApprovalSettings</span></span>|[<span data-ttu-id="229cb-174">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="229cb-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="229cb-175">Quem deve aprovar solicitações de pacote do Access nessa política.</span><span class="sxs-lookup"><span data-stu-id="229cb-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="229cb-176">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="229cb-176">requestorSettings</span></span>|[<span data-ttu-id="229cb-177">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="229cb-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="229cb-178">Quem pode solicitar esse pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="229cb-178">Who can request this access package from this policy.</span></span>|
|<span data-ttu-id="229cb-179">algumas</span><span class="sxs-lookup"><span data-stu-id="229cb-179">questions</span></span>|<span data-ttu-id="229cb-180">coleção [accessPackageQuestion](accesspackagequestion.md)</span><span class="sxs-lookup"><span data-stu-id="229cb-180">[accessPackageQuestion](accesspackagequestion.md) collection</span></span>|<span data-ttu-id="229cb-181">Perguntas que são representadas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="229cb-181">Questions that are posed to the  requestor.</span></span>|


## <a name="relationships"></a><span data-ttu-id="229cb-182">Relações</span><span class="sxs-lookup"><span data-stu-id="229cb-182">Relationships</span></span>

| <span data-ttu-id="229cb-183">Relação</span><span class="sxs-lookup"><span data-stu-id="229cb-183">Relationship</span></span> | <span data-ttu-id="229cb-184">Tipo</span><span class="sxs-lookup"><span data-stu-id="229cb-184">Type</span></span>        | <span data-ttu-id="229cb-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="229cb-185">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="229cb-186">accessPackage</span><span class="sxs-lookup"><span data-stu-id="229cb-186">accessPackage</span></span>|[<span data-ttu-id="229cb-187">accessPackage</span><span class="sxs-lookup"><span data-stu-id="229cb-187">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="229cb-188">O pacote de acesso com esta política.</span><span class="sxs-lookup"><span data-stu-id="229cb-188">The access package with this policy.</span></span> <span data-ttu-id="229cb-189">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="229cb-189">Read-only.</span></span> <span data-ttu-id="229cb-190">Anulável.</span><span class="sxs-lookup"><span data-stu-id="229cb-190">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="229cb-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="229cb-191">JSON representation</span></span>

<span data-ttu-id="229cb-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="229cb-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "baseType": "",
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

