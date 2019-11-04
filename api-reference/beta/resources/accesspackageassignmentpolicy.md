---
title: tipo de recurso accessPackageAssignmentPolicy
description: Uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: acb7c7b355d2a03d78cad1127882f272135fc4a2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939205"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a><span data-ttu-id="54567-103">tipo de recurso accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="54567-103">accessPackageAssignmentPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54567-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma política de atribuição de pacote do Access especifica a política pela qual as entidades podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="54567-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment policy specifies the policy by which subjects can request or be assigned an access package via an access package assignment.</span></span> <span data-ttu-id="54567-105">Um pacote de acesso pode ter zero ou mais políticas.</span><span class="sxs-lookup"><span data-stu-id="54567-105">An access package can have zero or more policies.</span></span> <span data-ttu-id="54567-106">Quando uma solicitação de um assunto é recebida, o assunto é correspondido em relação a cada política para localizar a política (se houver) desse assunto.</span><span class="sxs-lookup"><span data-stu-id="54567-106">When a request from a subject is received, the subject is matched against each policy to find the policy (if any) for that subject.</span></span> <span data-ttu-id="54567-107">A política determina se a solicitação requer aprovação e a duração da atribuição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="54567-107">The policy then determines whether the request requires approval, and the duration of the access package assignment.</span></span>

<span data-ttu-id="54567-108">Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="54567-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) which references the access package and access package assignment policy.</span></span>


## <a name="methods"></a><span data-ttu-id="54567-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="54567-109">Methods</span></span>

| <span data-ttu-id="54567-110">Método</span><span class="sxs-lookup"><span data-stu-id="54567-110">Method</span></span>       | <span data-ttu-id="54567-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="54567-111">Return Type</span></span> | <span data-ttu-id="54567-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="54567-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="54567-113">Listar accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="54567-113">List accessPackageAssignmentPolicies</span></span>](../api/accesspackageassignmentpolicy-list.md) | <span data-ttu-id="54567-114">coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="54567-114">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span> | <span data-ttu-id="54567-115">Recupere uma lista de objetos accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="54567-115">Retrieve a list of accessPackageAssignmentPolicy objects.</span></span> |
| [<span data-ttu-id="54567-116">Criar accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="54567-116">Create accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-post.md) | [<span data-ttu-id="54567-117">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="54567-117">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="54567-118">Criar um novo objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="54567-118">Create a new accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="54567-119">Obter accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="54567-119">Get accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-get.md) | [<span data-ttu-id="54567-120">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="54567-120">accessPackageAssignmentPolicy</span></span>](accesspackageassignmentpolicy.md) | <span data-ttu-id="54567-121">Ler propriedades e relações de um objeto accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="54567-121">Read properties and relationships of an accessPackageAssignmentPolicy object.</span></span> |
| [<span data-ttu-id="54567-122">Excluir accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="54567-122">Delete accessPackageAssignmentPolicy</span></span>](../api/accesspackageassignmentpolicy-delete.md) | | <span data-ttu-id="54567-123">Excluir um accessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="54567-123">Delete an accessPackageAssignmentPolicy.</span></span> |

## <a name="properties"></a><span data-ttu-id="54567-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54567-124">Properties</span></span>

| <span data-ttu-id="54567-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54567-125">Property</span></span>     | <span data-ttu-id="54567-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="54567-126">Type</span></span>        | <span data-ttu-id="54567-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="54567-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54567-128">accessPackageId</span><span class="sxs-lookup"><span data-stu-id="54567-128">accessPackageId</span></span>|<span data-ttu-id="54567-129">String</span><span class="sxs-lookup"><span data-stu-id="54567-129">String</span></span>|<span data-ttu-id="54567-130">ID do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="54567-130">ID of the access package.</span></span>|
|<span data-ttu-id="54567-131">exextend</span><span class="sxs-lookup"><span data-stu-id="54567-131">canExtend</span></span>|<span data-ttu-id="54567-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="54567-132">Boolean</span></span>|<span data-ttu-id="54567-133">Indica se um usuário pode estender a duração da atribuição de pacote de acesso após a aprovação.</span><span class="sxs-lookup"><span data-stu-id="54567-133">Indicates whether a user can extend the access package assignment duration after approval.</span></span>|
|<span data-ttu-id="54567-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="54567-134">createdBy</span></span>|<span data-ttu-id="54567-135">String</span><span class="sxs-lookup"><span data-stu-id="54567-135">String</span></span>|<span data-ttu-id="54567-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54567-136">Read-only.</span></span>|
|<span data-ttu-id="54567-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54567-137">createdDateTime</span></span>|<span data-ttu-id="54567-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54567-138">DateTimeOffset</span></span>|<span data-ttu-id="54567-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="54567-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="54567-141">description</span><span class="sxs-lookup"><span data-stu-id="54567-141">description</span></span>|<span data-ttu-id="54567-142">String</span><span class="sxs-lookup"><span data-stu-id="54567-142">String</span></span>|<span data-ttu-id="54567-143">A descrição da política.</span><span class="sxs-lookup"><span data-stu-id="54567-143">The description of the policy.</span></span>|
|<span data-ttu-id="54567-144">displayName</span><span class="sxs-lookup"><span data-stu-id="54567-144">displayName</span></span>|<span data-ttu-id="54567-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54567-145">String</span></span>|<span data-ttu-id="54567-146">O nome de exibição da política.</span><span class="sxs-lookup"><span data-stu-id="54567-146">The display name of the policy.</span></span>|
|<span data-ttu-id="54567-147">durationInDays</span><span class="sxs-lookup"><span data-stu-id="54567-147">durationInDays</span></span>|<span data-ttu-id="54567-148">Int32</span><span class="sxs-lookup"><span data-stu-id="54567-148">Int32</span></span>|<span data-ttu-id="54567-149">O número de dias em que as atribuições dessa política duram até que tenham expirado.</span><span class="sxs-lookup"><span data-stu-id="54567-149">The number of days in which assignments from this policy last until they are expired.</span></span>|
|<span data-ttu-id="54567-150">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="54567-150">expirationDateTime</span></span>|<span data-ttu-id="54567-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54567-151">DateTimeOffset</span></span>|<span data-ttu-id="54567-152">A data de validade das atribuições criadas nesta política.</span><span class="sxs-lookup"><span data-stu-id="54567-152">The expiration date for assignments created in this policy.</span></span> <span data-ttu-id="54567-153">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="54567-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="54567-154">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="54567-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="54567-155">id</span><span class="sxs-lookup"><span data-stu-id="54567-155">id</span></span>|<span data-ttu-id="54567-156">String</span><span class="sxs-lookup"><span data-stu-id="54567-156">String</span></span>| <span data-ttu-id="54567-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54567-157">Read-only.</span></span>|
|<span data-ttu-id="54567-158">isEnabled</span><span class="sxs-lookup"><span data-stu-id="54567-158">isEnabled</span></span>|<span data-ttu-id="54567-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="54567-159">Boolean</span></span>|<span data-ttu-id="54567-160">Essa política pode ser usada para novas solicitações.</span><span class="sxs-lookup"><span data-stu-id="54567-160">Can this policy be used for new requests.</span></span>|
|<span data-ttu-id="54567-161">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="54567-161">modifiedBy</span></span>|<span data-ttu-id="54567-162">String</span><span class="sxs-lookup"><span data-stu-id="54567-162">String</span></span>|<span data-ttu-id="54567-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54567-163">Read-only.</span></span>|
|<span data-ttu-id="54567-164">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54567-164">modifiedDateTime</span></span>|<span data-ttu-id="54567-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54567-165">DateTimeOffset</span></span>|<span data-ttu-id="54567-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="54567-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="54567-168">Relações</span><span class="sxs-lookup"><span data-stu-id="54567-168">Relationships</span></span>

| <span data-ttu-id="54567-169">Relação</span><span class="sxs-lookup"><span data-stu-id="54567-169">Relationship</span></span> | <span data-ttu-id="54567-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="54567-170">Type</span></span>        | <span data-ttu-id="54567-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="54567-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54567-172">accessPackage</span><span class="sxs-lookup"><span data-stu-id="54567-172">accessPackage</span></span>|[<span data-ttu-id="54567-173">accessPackage</span><span class="sxs-lookup"><span data-stu-id="54567-173">accessPackage</span></span>](accesspackage.md)| <span data-ttu-id="54567-174">O pacote de acesso com esta política.</span><span class="sxs-lookup"><span data-stu-id="54567-174">The access package with this policy.</span></span> <span data-ttu-id="54567-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54567-175">Read-only.</span></span> <span data-ttu-id="54567-176">Anulável.</span><span class="sxs-lookup"><span data-stu-id="54567-176">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54567-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54567-177">JSON representation</span></span>

<span data-ttu-id="54567-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54567-178">The following is a JSON representation of the resource.</span></span>

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
    "isEnabled": false,
    "canExtend": false,
    "durationInDays": 365
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
