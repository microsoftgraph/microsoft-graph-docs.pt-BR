---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3446b637835facfbe9a03e31dbdb8e9421b2faed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030503"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="0ee50-103">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="0ee50-103">educationSchool resource type</span></span>

<span data-ttu-id="0ee50-104">Recurso usado para gerenciar aulas, professores e alunos da escola representada.</span><span class="sxs-lookup"><span data-stu-id="0ee50-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="0ee50-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0ee50-105">Methods</span></span>

| <span data-ttu-id="0ee50-106">Método</span><span class="sxs-lookup"><span data-stu-id="0ee50-106">Method</span></span>           | <span data-ttu-id="0ee50-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0ee50-107">Return Type</span></span>    |<span data-ttu-id="0ee50-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ee50-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ee50-109">Get</span><span class="sxs-lookup"><span data-stu-id="0ee50-109">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="0ee50-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="0ee50-110">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="0ee50-111">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="0ee50-111">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="0ee50-112">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="0ee50-112">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="0ee50-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="0ee50-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="0ee50-114">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="0ee50-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="0ee50-115">Listar classes</span><span class="sxs-lookup"><span data-stu-id="0ee50-115">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="0ee50-116">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="0ee50-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="0ee50-117">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="0ee50-117">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="0ee50-118">Remover classe</span><span class="sxs-lookup"><span data-stu-id="0ee50-118">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="0ee50-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="0ee50-119">educationClass</span></span>](educationclass.md)| <span data-ttu-id="0ee50-120">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="0ee50-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="0ee50-121">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="0ee50-121">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="0ee50-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="0ee50-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="0ee50-123">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="0ee50-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="0ee50-124">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="0ee50-124">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="0ee50-125">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="0ee50-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="0ee50-126">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="0ee50-126">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="0ee50-127">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="0ee50-127">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="0ee50-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="0ee50-128">educationUser</span></span>](educationuser.md)| <span data-ttu-id="0ee50-129">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="0ee50-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="0ee50-130">Atualizar</span><span class="sxs-lookup"><span data-stu-id="0ee50-130">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="0ee50-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="0ee50-131">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="0ee50-132">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="0ee50-132">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="0ee50-133">Delete</span><span class="sxs-lookup"><span data-stu-id="0ee50-133">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="0ee50-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ee50-134">None</span></span> |<span data-ttu-id="0ee50-135">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="0ee50-135">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0ee50-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ee50-136">Properties</span></span>
| <span data-ttu-id="0ee50-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ee50-137">Property</span></span>     | <span data-ttu-id="0ee50-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ee50-138">Type</span></span>   |<span data-ttu-id="0ee50-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ee50-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ee50-140">id</span><span class="sxs-lookup"><span data-stu-id="0ee50-140">id</span></span>|<span data-ttu-id="0ee50-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ee50-141">String</span></span>|<span data-ttu-id="0ee50-142">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-142">GUID of this school.</span></span>|
|<span data-ttu-id="0ee50-143">displayName</span><span class="sxs-lookup"><span data-stu-id="0ee50-143">displayName</span></span>| <span data-ttu-id="0ee50-144">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-144">String</span></span>| <span data-ttu-id="0ee50-145">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-145">Display name of the school.</span></span>| 
|<span data-ttu-id="0ee50-146">descrição</span><span class="sxs-lookup"><span data-stu-id="0ee50-146">description</span></span>| <span data-ttu-id="0ee50-147">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-147">String</span></span> | <span data-ttu-id="0ee50-148">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-148">Description of the school.</span></span>| 
|<span data-ttu-id="0ee50-149">status</span><span class="sxs-lookup"><span data-stu-id="0ee50-149">status</span></span>| <span data-ttu-id="0ee50-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ee50-150">string</span></span>| <span data-ttu-id="0ee50-151">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0ee50-151">Read-Only.</span></span> <span data-ttu-id="0ee50-152">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="0ee50-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="0ee50-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="0ee50-153">externalSource</span></span>| <span data-ttu-id="0ee50-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="0ee50-154">educationExternalSource</span></span>| <span data-ttu-id="0ee50-155">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0ee50-155">Read-Only.</span></span>  <span data-ttu-id="0ee50-156">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0ee50-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0ee50-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="0ee50-157">principalEmail</span></span>| <span data-ttu-id="0ee50-158">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-158">String</span></span>| <span data-ttu-id="0ee50-159">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="0ee50-159">Email address of the principal.</span></span>|
|<span data-ttu-id="0ee50-160">principalName</span><span class="sxs-lookup"><span data-stu-id="0ee50-160">principalName</span></span>| <span data-ttu-id="0ee50-161">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-161">String</span></span> | <span data-ttu-id="0ee50-162">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="0ee50-162">Name of the principal.</span></span>|
|<span data-ttu-id="0ee50-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="0ee50-163">externalPrincipalId</span></span>| <span data-ttu-id="0ee50-164">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-164">String</span></span> | <span data-ttu-id="0ee50-165">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0ee50-165">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="0ee50-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="0ee50-166">highestGrade</span></span>|<span data-ttu-id="0ee50-167">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-167">String</span></span>| <span data-ttu-id="0ee50-168">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="0ee50-168">Highest grade taught.</span></span> |
|<span data-ttu-id="0ee50-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="0ee50-169">lowestGrade</span></span>|<span data-ttu-id="0ee50-170">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-170">String</span></span>| <span data-ttu-id="0ee50-171">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="0ee50-171">Lowest grade taught.</span></span> |
|<span data-ttu-id="0ee50-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="0ee50-172">schoolNumber</span></span>|<span data-ttu-id="0ee50-173">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-173">String</span></span>| <span data-ttu-id="0ee50-174">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-174">School Number.</span></span>|
|<span data-ttu-id="0ee50-175">externalId</span><span class="sxs-lookup"><span data-stu-id="0ee50-175">externalId</span></span>|<span data-ttu-id="0ee50-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ee50-176">String</span></span>| <span data-ttu-id="0ee50-177">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0ee50-177">ID of school in syncing system.</span></span> |
|<span data-ttu-id="0ee50-178">phone</span><span class="sxs-lookup"><span data-stu-id="0ee50-178">phone</span></span>|<span data-ttu-id="0ee50-179">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-179">String</span></span>| <span data-ttu-id="0ee50-180">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-180">Phone number of school.</span></span> |
|<span data-ttu-id="0ee50-181">fax</span><span class="sxs-lookup"><span data-stu-id="0ee50-181">fax</span></span>|<span data-ttu-id="0ee50-182">String</span><span class="sxs-lookup"><span data-stu-id="0ee50-182">String</span></span>| <span data-ttu-id="0ee50-183">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-183">Fax number of school.</span></span> |
|<span data-ttu-id="0ee50-184">address</span><span class="sxs-lookup"><span data-stu-id="0ee50-184">address</span></span>|[<span data-ttu-id="0ee50-185">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="0ee50-185">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="0ee50-186">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-186">Address of the school.</span></span>|
|<span data-ttu-id="0ee50-187">createdBy</span><span class="sxs-lookup"><span data-stu-id="0ee50-187">createdBy</span></span>|[<span data-ttu-id="0ee50-188">identitySet</span><span class="sxs-lookup"><span data-stu-id="0ee50-188">identitySet</span></span>](identityset.md)|<span data-ttu-id="0ee50-189">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-189">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ee50-190">Relações</span><span class="sxs-lookup"><span data-stu-id="0ee50-190">Relationships</span></span>
| <span data-ttu-id="0ee50-191">Relação</span><span class="sxs-lookup"><span data-stu-id="0ee50-191">Relationship</span></span> | <span data-ttu-id="0ee50-192">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ee50-192">Type</span></span>   |<span data-ttu-id="0ee50-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ee50-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ee50-194">classes</span><span class="sxs-lookup"><span data-stu-id="0ee50-194">classes</span></span>|<span data-ttu-id="0ee50-195">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="0ee50-195">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="0ee50-196">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-196">Classes taught at the school.</span></span> <span data-ttu-id="0ee50-197">Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ee50-197">Nullable.</span></span>|
|<span data-ttu-id="0ee50-198">users</span><span class="sxs-lookup"><span data-stu-id="0ee50-198">users</span></span>|<span data-ttu-id="0ee50-199">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="0ee50-199">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="0ee50-200">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="0ee50-200">Users in the school.</span></span> <span data-ttu-id="0ee50-201">Anulável.</span><span class="sxs-lookup"><span data-stu-id="0ee50-201">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ee50-202">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ee50-202">JSON representation</span></span>

<span data-ttu-id="0ee50-203">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ee50-203">The following is a JSON representation of the resource.</span></span>

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
