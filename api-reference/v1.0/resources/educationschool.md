---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2549d8babd000a36f0ff3ccd38541ef3c1b2e466
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463667"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="7156d-103">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="7156d-103">educationSchool resource type</span></span>

<span data-ttu-id="7156d-104">Recurso usado para gerenciar aulas, professores e alunos da escola representada.</span><span class="sxs-lookup"><span data-stu-id="7156d-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="7156d-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7156d-105">Methods</span></span>

| <span data-ttu-id="7156d-106">Método</span><span class="sxs-lookup"><span data-stu-id="7156d-106">Method</span></span>           | <span data-ttu-id="7156d-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7156d-107">Return Type</span></span>    |<span data-ttu-id="7156d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7156d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7156d-109">Obter</span><span class="sxs-lookup"><span data-stu-id="7156d-109">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="7156d-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="7156d-110">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="7156d-111">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="7156d-111">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="7156d-112">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="7156d-112">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="7156d-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="7156d-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="7156d-114">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="7156d-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="7156d-115">Listar classes</span><span class="sxs-lookup"><span data-stu-id="7156d-115">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="7156d-116">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="7156d-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="7156d-117">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="7156d-117">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="7156d-118">Remover classe</span><span class="sxs-lookup"><span data-stu-id="7156d-118">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="7156d-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="7156d-119">educationClass</span></span>](educationclass.md)| <span data-ttu-id="7156d-120">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="7156d-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="7156d-121">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="7156d-121">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="7156d-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="7156d-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="7156d-123">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="7156d-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="7156d-124">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="7156d-124">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="7156d-125">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="7156d-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="7156d-126">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="7156d-126">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="7156d-127">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="7156d-127">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="7156d-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="7156d-128">educationUser</span></span>](educationuser.md)| <span data-ttu-id="7156d-129">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="7156d-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="7156d-130">Atualizar</span><span class="sxs-lookup"><span data-stu-id="7156d-130">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="7156d-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="7156d-131">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="7156d-132">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="7156d-132">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="7156d-133">Excluir</span><span class="sxs-lookup"><span data-stu-id="7156d-133">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="7156d-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7156d-134">None</span></span> |<span data-ttu-id="7156d-135">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="7156d-135">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7156d-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7156d-136">Properties</span></span>
| <span data-ttu-id="7156d-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7156d-137">Property</span></span>     | <span data-ttu-id="7156d-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="7156d-138">Type</span></span>   |<span data-ttu-id="7156d-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7156d-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7156d-140">id</span><span class="sxs-lookup"><span data-stu-id="7156d-140">id</span></span>|<span data-ttu-id="7156d-141">String</span><span class="sxs-lookup"><span data-stu-id="7156d-141">String</span></span>|<span data-ttu-id="7156d-142">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-142">GUID of this school.</span></span>|
|<span data-ttu-id="7156d-143">displayName</span><span class="sxs-lookup"><span data-stu-id="7156d-143">displayName</span></span>| <span data-ttu-id="7156d-144">String</span><span class="sxs-lookup"><span data-stu-id="7156d-144">String</span></span>| <span data-ttu-id="7156d-145">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-145">Display name of the school.</span></span>| 
|<span data-ttu-id="7156d-146">description</span><span class="sxs-lookup"><span data-stu-id="7156d-146">description</span></span>| <span data-ttu-id="7156d-147">String</span><span class="sxs-lookup"><span data-stu-id="7156d-147">String</span></span> | <span data-ttu-id="7156d-148">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-148">Description of the school.</span></span>| 
|<span data-ttu-id="7156d-149">status</span><span class="sxs-lookup"><span data-stu-id="7156d-149">status</span></span>| <span data-ttu-id="7156d-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7156d-150">string</span></span>| <span data-ttu-id="7156d-151">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="7156d-151">Read-Only.</span></span> <span data-ttu-id="7156d-152">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="7156d-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="7156d-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="7156d-153">externalSource</span></span>| <span data-ttu-id="7156d-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="7156d-154">educationExternalSource</span></span>| <span data-ttu-id="7156d-155">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="7156d-155">Read-Only.</span></span>  <span data-ttu-id="7156d-156">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7156d-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7156d-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="7156d-157">principalEmail</span></span>| <span data-ttu-id="7156d-158">String</span><span class="sxs-lookup"><span data-stu-id="7156d-158">String</span></span>| <span data-ttu-id="7156d-159">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="7156d-159">Email address of the principal.</span></span>|
|<span data-ttu-id="7156d-160">principalName</span><span class="sxs-lookup"><span data-stu-id="7156d-160">principalName</span></span>| <span data-ttu-id="7156d-161">String</span><span class="sxs-lookup"><span data-stu-id="7156d-161">String</span></span> | <span data-ttu-id="7156d-162">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="7156d-162">Name of the principal.</span></span>|
|<span data-ttu-id="7156d-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="7156d-163">externalPrincipalId</span></span>| <span data-ttu-id="7156d-164">String</span><span class="sxs-lookup"><span data-stu-id="7156d-164">String</span></span> | <span data-ttu-id="7156d-165">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7156d-165">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="7156d-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="7156d-166">highestGrade</span></span>|<span data-ttu-id="7156d-167">String</span><span class="sxs-lookup"><span data-stu-id="7156d-167">String</span></span>| <span data-ttu-id="7156d-168">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="7156d-168">Highest grade taught.</span></span> |
|<span data-ttu-id="7156d-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="7156d-169">lowestGrade</span></span>|<span data-ttu-id="7156d-170">String</span><span class="sxs-lookup"><span data-stu-id="7156d-170">String</span></span>| <span data-ttu-id="7156d-171">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="7156d-171">Lowest grade taught.</span></span> |
|<span data-ttu-id="7156d-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="7156d-172">schoolNumber</span></span>|<span data-ttu-id="7156d-173">String</span><span class="sxs-lookup"><span data-stu-id="7156d-173">String</span></span>| <span data-ttu-id="7156d-174">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-174">School Number.</span></span>|
|<span data-ttu-id="7156d-175">externalId</span><span class="sxs-lookup"><span data-stu-id="7156d-175">externalId</span></span>|<span data-ttu-id="7156d-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7156d-176">String</span></span>| <span data-ttu-id="7156d-177">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7156d-177">ID of school in syncing system.</span></span> |
|<span data-ttu-id="7156d-178">phone</span><span class="sxs-lookup"><span data-stu-id="7156d-178">phone</span></span>|<span data-ttu-id="7156d-179">String</span><span class="sxs-lookup"><span data-stu-id="7156d-179">String</span></span>| <span data-ttu-id="7156d-180">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-180">Phone number of school.</span></span> |
|<span data-ttu-id="7156d-181">fax</span><span class="sxs-lookup"><span data-stu-id="7156d-181">fax</span></span>|<span data-ttu-id="7156d-182">String</span><span class="sxs-lookup"><span data-stu-id="7156d-182">String</span></span>| <span data-ttu-id="7156d-183">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-183">Fax number of school.</span></span> |
|<span data-ttu-id="7156d-184">address</span><span class="sxs-lookup"><span data-stu-id="7156d-184">address</span></span>|[<span data-ttu-id="7156d-185">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="7156d-185">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="7156d-186">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-186">Address of the school.</span></span>|
|<span data-ttu-id="7156d-187">createdBy</span><span class="sxs-lookup"><span data-stu-id="7156d-187">createdBy</span></span>|[<span data-ttu-id="7156d-188">identitySet</span><span class="sxs-lookup"><span data-stu-id="7156d-188">identitySet</span></span>](identityset.md)|<span data-ttu-id="7156d-189">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-189">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7156d-190">Relações</span><span class="sxs-lookup"><span data-stu-id="7156d-190">Relationships</span></span>
| <span data-ttu-id="7156d-191">Relação</span><span class="sxs-lookup"><span data-stu-id="7156d-191">Relationship</span></span> | <span data-ttu-id="7156d-192">Tipo</span><span class="sxs-lookup"><span data-stu-id="7156d-192">Type</span></span>   |<span data-ttu-id="7156d-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="7156d-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7156d-194">classes</span><span class="sxs-lookup"><span data-stu-id="7156d-194">classes</span></span>|<span data-ttu-id="7156d-195">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="7156d-195">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="7156d-196">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-196">Classes taught at the school.</span></span> <span data-ttu-id="7156d-197">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7156d-197">Nullable.</span></span>|
|<span data-ttu-id="7156d-198">users</span><span class="sxs-lookup"><span data-stu-id="7156d-198">users</span></span>|<span data-ttu-id="7156d-199">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="7156d-199">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="7156d-200">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="7156d-200">Users in the school.</span></span> <span data-ttu-id="7156d-201">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7156d-201">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7156d-202">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7156d-202">JSON representation</span></span>

<span data-ttu-id="7156d-203">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7156d-203">The following is a JSON representation of the resource.</span></span>

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
