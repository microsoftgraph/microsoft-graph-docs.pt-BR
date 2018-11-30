---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
ms.openlocfilehash: 8a87b3a0ceebf9a3dd66978da1bdde2d677ef63e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007148"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="dbea5-103">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="dbea5-103">educationSchool resource type</span></span>

<span data-ttu-id="dbea5-104">Recurso usado para gerenciar aulas, professores e alunos da escola representada.</span><span class="sxs-lookup"><span data-stu-id="dbea5-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="dbea5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="dbea5-105">Methods</span></span>

| <span data-ttu-id="dbea5-106">Método</span><span class="sxs-lookup"><span data-stu-id="dbea5-106">Method</span></span>           | <span data-ttu-id="dbea5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dbea5-107">Return Type</span></span>    |<span data-ttu-id="dbea5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbea5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dbea5-109">Obter</span><span class="sxs-lookup"><span data-stu-id="dbea5-109">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="dbea5-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="dbea5-110">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="dbea5-111">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="dbea5-111">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="dbea5-112">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="dbea5-112">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="dbea5-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="dbea5-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="dbea5-114">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="dbea5-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="dbea5-115">Listar classes</span><span class="sxs-lookup"><span data-stu-id="dbea5-115">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="dbea5-116">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="dbea5-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="dbea5-117">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="dbea5-117">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="dbea5-118">Remover classe</span><span class="sxs-lookup"><span data-stu-id="dbea5-118">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="dbea5-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="dbea5-119">educationClass</span></span>](educationclass.md)| <span data-ttu-id="dbea5-120">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="dbea5-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="dbea5-121">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="dbea5-121">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="dbea5-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="dbea5-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="dbea5-123">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="dbea5-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="dbea5-124">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="dbea5-124">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="dbea5-125">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="dbea5-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="dbea5-126">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="dbea5-126">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="dbea5-127">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="dbea5-127">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="dbea5-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="dbea5-128">educationUser</span></span>](educationuser.md)| <span data-ttu-id="dbea5-129">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="dbea5-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="dbea5-130">Atualizar</span><span class="sxs-lookup"><span data-stu-id="dbea5-130">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="dbea5-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="dbea5-131">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="dbea5-132">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="dbea5-132">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="dbea5-133">Excluir</span><span class="sxs-lookup"><span data-stu-id="dbea5-133">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="dbea5-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dbea5-134">None</span></span> |<span data-ttu-id="dbea5-135">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="dbea5-135">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dbea5-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbea5-136">Properties</span></span>
| <span data-ttu-id="dbea5-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbea5-137">Property</span></span>     | <span data-ttu-id="dbea5-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbea5-138">Type</span></span>   |<span data-ttu-id="dbea5-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbea5-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbea5-140">id</span><span class="sxs-lookup"><span data-stu-id="dbea5-140">id</span></span>|<span data-ttu-id="dbea5-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-141">String</span></span>|<span data-ttu-id="dbea5-142">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-142">GUID of this school.</span></span>|
|<span data-ttu-id="dbea5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="dbea5-143">displayName</span></span>| <span data-ttu-id="dbea5-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-144">String</span></span>| <span data-ttu-id="dbea5-145">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-145">Display name of the school.</span></span>| 
|<span data-ttu-id="dbea5-146">description</span><span class="sxs-lookup"><span data-stu-id="dbea5-146">description</span></span>| <span data-ttu-id="dbea5-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-147">String</span></span> | <span data-ttu-id="dbea5-148">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-148">Description of the school.</span></span>| 
|<span data-ttu-id="dbea5-149">status</span><span class="sxs-lookup"><span data-stu-id="dbea5-149">status</span></span>| <span data-ttu-id="dbea5-150">string</span><span class="sxs-lookup"><span data-stu-id="dbea5-150">string</span></span>| <span data-ttu-id="dbea5-151">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="dbea5-151">Read-Only.</span></span> <span data-ttu-id="dbea5-152">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="dbea5-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="dbea5-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="dbea5-153">externalSource</span></span>| <span data-ttu-id="dbea5-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="dbea5-154">educationExternalSource</span></span>| <span data-ttu-id="dbea5-155">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="dbea5-155">Read-Only.</span></span>  <span data-ttu-id="dbea5-156">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dbea5-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dbea5-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="dbea5-157">principalEmail</span></span>| <span data-ttu-id="dbea5-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-158">String</span></span>| <span data-ttu-id="dbea5-159">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="dbea5-159">Email address of the principal.</span></span>|
|<span data-ttu-id="dbea5-160">principalName</span><span class="sxs-lookup"><span data-stu-id="dbea5-160">principalName</span></span>| <span data-ttu-id="dbea5-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-161">String</span></span> | <span data-ttu-id="dbea5-162">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="dbea5-162">Name of the principal.</span></span>|
|<span data-ttu-id="dbea5-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="dbea5-163">externalPrincipalId</span></span>| <span data-ttu-id="dbea5-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-164">String</span></span> | <span data-ttu-id="dbea5-165">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="dbea5-165">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="dbea5-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="dbea5-166">highestGrade</span></span>|<span data-ttu-id="dbea5-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-167">String</span></span>| <span data-ttu-id="dbea5-168">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="dbea5-168">Highest grade taught.</span></span> |
|<span data-ttu-id="dbea5-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="dbea5-169">lowestGrade</span></span>|<span data-ttu-id="dbea5-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-170">String</span></span>| <span data-ttu-id="dbea5-171">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="dbea5-171">Lowest grade taught.</span></span> |
|<span data-ttu-id="dbea5-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="dbea5-172">schoolNumber</span></span>|<span data-ttu-id="dbea5-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-173">String</span></span>| <span data-ttu-id="dbea5-174">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-174">School Number.</span></span>|
|<span data-ttu-id="dbea5-175">externalId</span><span class="sxs-lookup"><span data-stu-id="dbea5-175">externalId</span></span>|<span data-ttu-id="dbea5-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-176">String</span></span>| <span data-ttu-id="dbea5-177">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="dbea5-177">ID of school in syncing system.</span></span> |
|<span data-ttu-id="dbea5-178">phone</span><span class="sxs-lookup"><span data-stu-id="dbea5-178">phone</span></span>|<span data-ttu-id="dbea5-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-179">String</span></span>| <span data-ttu-id="dbea5-180">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-180">Phone number of school.</span></span> |
|<span data-ttu-id="dbea5-181">fax</span><span class="sxs-lookup"><span data-stu-id="dbea5-181">fax</span></span>|<span data-ttu-id="dbea5-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbea5-182">String</span></span>| <span data-ttu-id="dbea5-183">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-183">Fax number of school.</span></span> |
|<span data-ttu-id="dbea5-184">address</span><span class="sxs-lookup"><span data-stu-id="dbea5-184">address</span></span>|[<span data-ttu-id="dbea5-185">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="dbea5-185">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="dbea5-186">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-186">Address of the school.</span></span>|
|<span data-ttu-id="dbea5-187">createdBy</span><span class="sxs-lookup"><span data-stu-id="dbea5-187">createdBy</span></span>|[<span data-ttu-id="dbea5-188">identitySet</span><span class="sxs-lookup"><span data-stu-id="dbea5-188">identitySet</span></span>](identityset.md)|<span data-ttu-id="dbea5-189">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-189">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbea5-190">Relações</span><span class="sxs-lookup"><span data-stu-id="dbea5-190">Relationships</span></span>
| <span data-ttu-id="dbea5-191">Relação</span><span class="sxs-lookup"><span data-stu-id="dbea5-191">Relationship</span></span> | <span data-ttu-id="dbea5-192">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbea5-192">Type</span></span>   |<span data-ttu-id="dbea5-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbea5-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbea5-194">classes</span><span class="sxs-lookup"><span data-stu-id="dbea5-194">classes</span></span>|<span data-ttu-id="dbea5-195">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="dbea5-195">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="dbea5-196">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-196">Classes taught at the school.</span></span> <span data-ttu-id="dbea5-197">Anulável.</span><span class="sxs-lookup"><span data-stu-id="dbea5-197">Nullable.</span></span>|
|<span data-ttu-id="dbea5-198">users</span><span class="sxs-lookup"><span data-stu-id="dbea5-198">users</span></span>|<span data-ttu-id="dbea5-199">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="dbea5-199">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="dbea5-200">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="dbea5-200">Users in the school.</span></span> <span data-ttu-id="dbea5-201">Anulável.</span><span class="sxs-lookup"><span data-stu-id="dbea5-201">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbea5-202">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbea5-202">JSON representation</span></span>

<span data-ttu-id="dbea5-203">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbea5-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
