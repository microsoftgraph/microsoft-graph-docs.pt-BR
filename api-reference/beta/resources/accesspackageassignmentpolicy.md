---
title: tipo de recurso accessPackageAssignmentPolicy
description: Uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 08fcefafe9a354a57415a7d05bee1ec57ffdc138
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331301"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="1ae1d-103">tipo de recurso accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="1ae1d-103">accessPackageAssignmentPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ae1d-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="1ae1d-105">Um pacote de acesso pode ter zero ou mais políticas.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-105">An access package can have zero or more policies.</span></span> <span data-ttu-id="1ae1d-106">Quando uma solicitação de um assunto é recebida, o assunto é correspondido em relação a cada política para localizar a política (se houver) com requestorSettings que inclua esse assunto.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-106">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) with requestorSettings that include that subject.</span></span> <span data-ttu-id="1ae1d-107">A política determina se a solicitação requer aprovação, a duração da atribuição do pacote de acesso e se a atribuição precisa ser revisada regularmente.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-107">The policy then determines whether the request requires approval, the duration of the access package assignment, and whether the assignment needs regularly review.</span></span>

<span data-ttu-id="1ae1d-108">Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="1ae1d-109">Methods</span><span class="sxs-lookup"><span data-stu-id="1ae1d-109">Methods</span></span>

| <span data-ttu-id="1ae1d-110">Método</span><span class="sxs-lookup"><span data-stu-id="1ae1d-110">Method</span></span>       | <span data-ttu-id="1ae1d-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1ae1d-111">Return Type</span></span> | <span data-ttu-id="1ae1d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ae1d-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1ae1d-113">Listar accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="1ae1d-113">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="1ae1d-114">coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1ae1d-114">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="1ae1d-115">Recupere uma lista de objetos accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-115">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="1ae1d-116">Criar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="1ae1d-116">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="1ae1d-117">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="1ae1d-117">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="1ae1d-118">Criar um novo objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-118">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="1ae1d-119">Obter accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="1ae1d-119">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="1ae1d-120">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="1ae1d-120">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="1ae1d-121">Ler propriedades e relações de um objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-121">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="1ae1d-122">Excluir accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="1ae1d-122">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="1ae1d-123">Excluir um accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-123">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="1ae1d-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ae1d-124">Properties</span></span>

| <span data-ttu-id="1ae1d-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ae1d-125">Property</span></span>     | <span data-ttu-id="1ae1d-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ae1d-126">Type</span></span>        | <span data-ttu-id="1ae1d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ae1d-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1ae1d-128">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="1ae1d-128">accessPackageId</span></span>|<span data-ttu-id="1ae1d-129">String</span><span class="sxs-lookup"><span data-stu-id="1ae1d-129">String</span></span>|<span data-ttu-id="1ae1d-130">ID do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-130">ID of the access package.</span></span>|
|<span data-ttu-id="1ae1d-131">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="1ae1d-131">accessReviewSettings</span></span>|[<span data-ttu-id="1ae1d-132">assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="1ae1d-132">assignmentReviewSettings</span></span>](assignmentreviewsettings.md)|<span data-ttu-id="1ae1d-133">Quem deve revisar e com que frequência as atribuições para o pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-133">Who must review, and how often, the assignments to the access package from this policy.</span></span> <span data-ttu-id="1ae1d-134">Essa propriedade será nula se as revisões não forem necessárias.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-134">This property is null if reviews are not required.</span></span>|
|<span data-ttu-id="1ae1d-135">exextend</span><span class="sxs-lookup"><span data-stu-id="1ae1d-135">canExtend</span></span>|<span data-ttu-id="1ae1d-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ae1d-136">Boolean</span></span>|<span data-ttu-id="1ae1d-137">Indica se um usuário pode estender a duração da atribuição de pacote de acesso após a aprovação.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-137">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="1ae1d-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="1ae1d-138">createdBy</span></span>|<span data-ttu-id="1ae1d-139">String</span><span class="sxs-lookup"><span data-stu-id="1ae1d-139">String</span></span>|<span data-ttu-id="1ae1d-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-140">Read-only.</span></span>|
|<span data-ttu-id="1ae1d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ae1d-141">createdDateTime</span></span>|<span data-ttu-id="1ae1d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ae1d-142">DateTimeOffset</span></span>|<span data-ttu-id="1ae1d-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1ae1d-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1ae1d-145">descrição</span><span class="sxs-lookup"><span data-stu-id="1ae1d-145">description</span></span>|<span data-ttu-id="1ae1d-146">String</span><span class="sxs-lookup"><span data-stu-id="1ae1d-146">String</span></span>|<span data-ttu-id="1ae1d-147">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-147">The description of the policy.</span></span>|
|<span data-ttu-id="1ae1d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="1ae1d-148">displayName</span></span>|<span data-ttu-id="1ae1d-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ae1d-149">String</span></span>|<span data-ttu-id="1ae1d-150">O nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-150">The display name of the policy.</span></span>|
|<span data-ttu-id="1ae1d-151">durationInDays</span><span class="sxs-lookup"><span data-stu-id="1ae1d-151">durationInDays</span></span>|<span data-ttu-id="1ae1d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1ae1d-152">Int32</span></span>|<span data-ttu-id="1ae1d-153">O número de dias em que as atribuições dessa política duram até que tenham expirado.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-153">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="1ae1d-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1ae1d-154">expirationDateTime</span></span>|<span data-ttu-id="1ae1d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ae1d-155">DateTimeOffset</span></span>|<span data-ttu-id="1ae1d-156">A data de validade das atribuições criadas nesta política.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-156">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="1ae1d-157">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1ae1d-158">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1ae1d-158">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1ae1d-159">id</span><span class="sxs-lookup"><span data-stu-id="1ae1d-159">id</span></span>|<span data-ttu-id="1ae1d-160">String</span><span class="sxs-lookup"><span data-stu-id="1ae1d-160">String</span></span>| <span data-ttu-id="1ae1d-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-161">Read-only.</span></span>|
|<span data-ttu-id="1ae1d-162">isDenyPolicy</span><span class="sxs-lookup"><span data-stu-id="1ae1d-162">isDenyPolicy</span></span>|<span data-ttu-id="1ae1d-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ae1d-163">Boolean</span></span>|<span data-ttu-id="1ae1d-164">Se true, a política não permitirá o acesso.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-164">If true, the policy will not permit access.</span></span> <span data-ttu-id="1ae1d-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-165">Read only.</span></span>|
|<span data-ttu-id="1ae1d-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="1ae1d-166">modifiedBy</span></span>|<span data-ttu-id="1ae1d-167">String</span><span class="sxs-lookup"><span data-stu-id="1ae1d-167">String</span></span>|<span data-ttu-id="1ae1d-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-168">Read-only.</span></span>|
|<span data-ttu-id="1ae1d-169">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ae1d-169">modifiedDateTime</span></span>|<span data-ttu-id="1ae1d-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ae1d-170">DateTimeOffset</span></span>|<span data-ttu-id="1ae1d-p106">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1ae1d-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1ae1d-173">requestApprovalSettings</span><span class="sxs-lookup"><span data-stu-id="1ae1d-173">requestApprovalSettings</span></span>|[<span data-ttu-id="1ae1d-174">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="1ae1d-174">approvalSettings</span></span>](approvalsettings.md)|<span data-ttu-id="1ae1d-175">Quem deve aprovar solicitações de pacote do Access nessa política.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-175">Who must approve requests for access package in this policy.</span></span>|
|<span data-ttu-id="1ae1d-176">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="1ae1d-176">requestorSettings</span></span>|[<span data-ttu-id="1ae1d-177">requestorSettings</span><span class="sxs-lookup"><span data-stu-id="1ae1d-177">requestorSettings</span></span>](requestorsettings.md)|<span data-ttu-id="1ae1d-178">Quem pode solicitar esse pacote de acesso desta política.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-178">Who can request this access package from this policy.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1ae1d-179">Relações</span><span class="sxs-lookup"><span data-stu-id="1ae1d-179">Relationships</span></span>

| <span data-ttu-id="1ae1d-180">Relação</span><span class="sxs-lookup"><span data-stu-id="1ae1d-180">Relationship</span></span> | <span data-ttu-id="1ae1d-181">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ae1d-181">Type</span></span>        | <span data-ttu-id="1ae1d-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ae1d-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1ae1d-183">accessPackage</span><span class="sxs-lookup"><span data-stu-id="1ae1d-183">accessPackage</span></span>|[<span data-ttu-id="1ae1d-184">accessPackage</span><span class="sxs-lookup"><span data-stu-id="1ae1d-184">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="1ae1d-185">O pacote de acesso com esta política.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-185">The access package with this policy.</span></span> <span data-ttu-id="1ae1d-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-186">Read-only.</span></span> <span data-ttu-id="1ae1d-187">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-187">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ae1d-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ae1d-188">JSON representation</span></span>

<span data-ttu-id="1ae1d-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ae1d-189">The following is a JSON representation of the resource.</span></span>

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
