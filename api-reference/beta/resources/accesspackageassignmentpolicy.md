---
title: tipo de recurso accessPackageAssignmentPolicy
description: Uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dd70512db17df29685c4af2d8aa4c410a78642b0
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534438"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="fc9f5-103">tipo de recurso accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="fc9f5-103">accessPackageAssignmentPolicy resource type</span></span>

<span data-ttu-id="fc9f5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fc9f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc9f5-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="fc9f5-106">Um pacote de acesso pode ter zero ou mais políticas.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-106">An access package can have zero or more policies.</span></span> <span data-ttu-id="fc9f5-107">Quando uma solicitação de um assunto é recebida, o assunto é correspondido em relação a cada política para localizar a política (se houver) com requestorSettings que inclua esse assunto.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-107">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="fc9f5-108">A política determina se a solicitação requer aprovação, a duração da atribuição do pacote de acesso e se a atribuição precisa ser revisada regularmente.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-108">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="fc9f5-109">Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-109">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="fc9f5-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc9f5-110">Methods</span></span>

| <span data-ttu-id="fc9f5-111">Método</span><span class="sxs-lookup"><span data-stu-id="fc9f5-111">Method</span></span>       | <span data-ttu-id="fc9f5-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc9f5-112">Return Type</span></span> | <span data-ttu-id="fc9f5-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc9f5-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fc9f5-114">Listar accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="fc9f5-114">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="fc9f5-115">coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fc9f5-115">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="fc9f5-116">Recupere uma lista de objetos accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-116">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="fc9f5-117">Criar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="fc9f5-117">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="fc9f5-118">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="fc9f5-118">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="fc9f5-119">Criar um novo objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-119">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="fc9f5-120">Obter accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="fc9f5-120">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="fc9f5-121">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="fc9f5-121">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="fc9f5-122">Ler propriedades e relações de um objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-122">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="fc9f5-123">Excluir accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="fc9f5-123">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="fc9f5-124">Excluir um accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-124">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc9f5-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc9f5-125">Properties</span></span>

| <span data-ttu-id="fc9f5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc9f5-126">Property</span></span>     | <span data-ttu-id="fc9f5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc9f5-127">Type</span></span>        | <span data-ttu-id="fc9f5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc9f5-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc9f5-129">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="fc9f5-129">accessPackageId</span></span>|<span data-ttu-id="fc9f5-130">String</span><span class="sxs-lookup"><span data-stu-id="fc9f5-130">String</span></span>|<span data-ttu-id="fc9f5-131">ID do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-131">ID of the access package.</span></span>|
|<span data-ttu-id="fc9f5-132">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="fc9f5-132">accessReviewSettings</span></span>|[<span data-ttu-id="fc9f5-133">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="fc9f5-133">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="fc9f5-134">Quem deve revisar e com que frequência as atribuições para o pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-134">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="fc9f5-135">Essa propriedade será nula se as revisões não forem necessárias.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-135">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="fc9f5-136">exextend</span><span class="sxs-lookup"><span data-stu-id="fc9f5-136">canExtend</span></span>|<span data-ttu-id="fc9f5-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc9f5-137">Boolean</span></span>|<span data-ttu-id="fc9f5-138">Indica se um usuário pode estender a duração da atribuição de pacote de acesso após a aprovação.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-138">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="fc9f5-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="fc9f5-139">createdBy</span></span>|<span data-ttu-id="fc9f5-140">String</span><span class="sxs-lookup"><span data-stu-id="fc9f5-140">String</span></span>|<span data-ttu-id="fc9f5-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-141">Read-only.</span></span>|
|<span data-ttu-id="fc9f5-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc9f5-142">createdDateTime</span></span>|<span data-ttu-id="fc9f5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc9f5-143">DateTimeOffset</span></span>|<span data-ttu-id="fc9f5-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fc9f5-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fc9f5-146">description</span><span class="sxs-lookup"><span data-stu-id="fc9f5-146">description</span></span>|<span data-ttu-id="fc9f5-147">String</span><span class="sxs-lookup"><span data-stu-id="fc9f5-147">String</span></span>|<span data-ttu-id="fc9f5-148">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-148">The description of the policy.</span></span>|
|<span data-ttu-id="fc9f5-149">displayName</span><span class="sxs-lookup"><span data-stu-id="fc9f5-149">displayName</span></span>|<span data-ttu-id="fc9f5-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc9f5-150">String</span></span>|<span data-ttu-id="fc9f5-151">O nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-151">The display name of the policy.</span></span>|
|<span data-ttu-id="fc9f5-152">durationInDays</span><span class="sxs-lookup"><span data-stu-id="fc9f5-152">durationInDays</span></span>|<span data-ttu-id="fc9f5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="fc9f5-153">Int32</span></span>|<span data-ttu-id="fc9f5-154">O número de dias em que as atribuições dessa política duram até que tenham expirado.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-154">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="fc9f5-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fc9f5-155">expirationDateTime</span></span>|<span data-ttu-id="fc9f5-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc9f5-156">DateTimeOffset</span></span>|<span data-ttu-id="fc9f5-157">A data de validade das atribuições criadas nesta política.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-157">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="fc9f5-158">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fc9f5-159">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fc9f5-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fc9f5-160">id</span><span class="sxs-lookup"><span data-stu-id="fc9f5-160">id</span></span>|<span data-ttu-id="fc9f5-161">String</span><span class="sxs-lookup"><span data-stu-id="fc9f5-161">String</span></span>| <span data-ttu-id="fc9f5-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-162">Read-only.</span></span>|
|<span data-ttu-id="fc9f5-163">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="fc9f5-163">modifiedBy</span></span>|<span data-ttu-id="fc9f5-164">String</span><span class="sxs-lookup"><span data-stu-id="fc9f5-164">String</span></span>|<span data-ttu-id="fc9f5-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-165">Read-only.</span></span>|
|<span data-ttu-id="fc9f5-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc9f5-166">modifiedDateTime</span></span>|<span data-ttu-id="fc9f5-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc9f5-167">DateTimeOffset</span></span>|<span data-ttu-id="fc9f5-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fc9f5-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fc9f5-170">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="fc9f5-170">requestApprovalSettings</span></span>|[<span data-ttu-id="fc9f5-171">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="fc9f5-171">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="fc9f5-172">Quem deve aprovar solicitações de pacote do Access nessa política.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-172">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="fc9f5-173">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="fc9f5-173">requestorSettings</span></span>|[<span data-ttu-id="fc9f5-174">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="fc9f5-174">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="fc9f5-175">Quem pode solicitar esse pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-175">Who can request this access package from this policy.</span></span>|


## <a name="relationships"></a><span data-ttu-id="fc9f5-176">Relações</span><span class="sxs-lookup"><span data-stu-id="fc9f5-176">Relationships</span></span>

| <span data-ttu-id="fc9f5-177">Relação</span><span class="sxs-lookup"><span data-stu-id="fc9f5-177">Relationship</span></span> | <span data-ttu-id="fc9f5-178">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc9f5-178">Type</span></span>        | <span data-ttu-id="fc9f5-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc9f5-179">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc9f5-180">accessPackage</span><span class="sxs-lookup"><span data-stu-id="fc9f5-180">accessPackage</span></span>|[<span data-ttu-id="fc9f5-181">accessPackage</span><span class="sxs-lookup"><span data-stu-id="fc9f5-181">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="fc9f5-182">O pacote de acesso com esta política.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-182">The access package with this policy.</span></span> <span data-ttu-id="fc9f5-183">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-183">Read-only.</span></span> <span data-ttu-id="fc9f5-184">Anulável.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc9f5-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc9f5-185">JSON representation</span></span>

<span data-ttu-id="fc9f5-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc9f5-186">The following is a JSON representation of the resource.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
