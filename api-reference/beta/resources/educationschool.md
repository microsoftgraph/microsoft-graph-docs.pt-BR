---
title: Tipo de recurso educationSchool
description: 'Escola A. O recurso **educationSchool** atualmente corresponde a um recurso administrativeUnit e compartilha a mesma ID.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512539"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="c9356-104">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="c9356-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9356-105">Escola A.</span><span class="sxs-lookup"><span data-stu-id="c9356-105">A school.</span></span> <span data-ttu-id="c9356-106">O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="c9356-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="c9356-107">Esse recurso é um subtipo de [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="c9356-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="c9356-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c9356-108">Methods</span></span>

| <span data-ttu-id="c9356-109">Método</span><span class="sxs-lookup"><span data-stu-id="c9356-109">Method</span></span>           | <span data-ttu-id="c9356-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c9356-110">Return Type</span></span>    |<span data-ttu-id="c9356-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9356-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9356-112">Obter</span><span class="sxs-lookup"><span data-stu-id="c9356-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="c9356-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="c9356-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="c9356-114">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="c9356-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="c9356-115">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="c9356-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="c9356-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="c9356-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="c9356-117">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="c9356-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="c9356-118">Listar classes</span><span class="sxs-lookup"><span data-stu-id="c9356-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="c9356-119">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="c9356-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="c9356-120">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="c9356-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="c9356-121">Remover classe</span><span class="sxs-lookup"><span data-stu-id="c9356-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="c9356-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="c9356-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="c9356-123">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="c9356-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="c9356-124">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="c9356-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="c9356-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="c9356-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c9356-126">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="c9356-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="c9356-127">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="c9356-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="c9356-128">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="c9356-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="c9356-129">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="c9356-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="c9356-130">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="c9356-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="c9356-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="c9356-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c9356-132">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="c9356-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="c9356-133">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c9356-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="c9356-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c9356-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="c9356-135">Obtenha a **administrativeUnit** que corresponde a essa **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="c9356-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="c9356-136">Atualizar</span><span class="sxs-lookup"><span data-stu-id="c9356-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="c9356-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="c9356-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="c9356-138">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="c9356-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="c9356-139">Excluir</span><span class="sxs-lookup"><span data-stu-id="c9356-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="c9356-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9356-140">None</span></span> |<span data-ttu-id="c9356-141">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="c9356-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c9356-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9356-142">Properties</span></span>
| <span data-ttu-id="c9356-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9356-143">Property</span></span>     | <span data-ttu-id="c9356-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9356-144">Type</span></span>   |<span data-ttu-id="c9356-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9356-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9356-146">id</span><span class="sxs-lookup"><span data-stu-id="c9356-146">id</span></span>|<span data-ttu-id="c9356-147">String</span><span class="sxs-lookup"><span data-stu-id="c9356-147">String</span></span>|<span data-ttu-id="c9356-148">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-148">GUID of this school.</span></span>|
|<span data-ttu-id="c9356-149">displayName</span><span class="sxs-lookup"><span data-stu-id="c9356-149">displayName</span></span>| <span data-ttu-id="c9356-150">String</span><span class="sxs-lookup"><span data-stu-id="c9356-150">String</span></span>| <span data-ttu-id="c9356-151">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-151">Display name of the school.</span></span>| 
|<span data-ttu-id="c9356-152">description</span><span class="sxs-lookup"><span data-stu-id="c9356-152">description</span></span>| <span data-ttu-id="c9356-153">String</span><span class="sxs-lookup"><span data-stu-id="c9356-153">String</span></span> | <span data-ttu-id="c9356-154">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-154">Description of the school.</span></span>| 
|<span data-ttu-id="c9356-155">status</span><span class="sxs-lookup"><span data-stu-id="c9356-155">status</span></span>| <span data-ttu-id="c9356-156">string</span><span class="sxs-lookup"><span data-stu-id="c9356-156">string</span></span>| <span data-ttu-id="c9356-157">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c9356-157">Read-Only.</span></span> <span data-ttu-id="c9356-158">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="c9356-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="c9356-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="c9356-159">externalSource</span></span>| <span data-ttu-id="c9356-160">string</span><span class="sxs-lookup"><span data-stu-id="c9356-160">string</span></span>| <span data-ttu-id="c9356-161">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c9356-161">Read-Only.</span></span>  <span data-ttu-id="c9356-162">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c9356-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c9356-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="c9356-163">principalEmail</span></span>| <span data-ttu-id="c9356-164">String</span><span class="sxs-lookup"><span data-stu-id="c9356-164">String</span></span>| <span data-ttu-id="c9356-165">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="c9356-165">Email address of the principal.</span></span>|
|<span data-ttu-id="c9356-166">principalName</span><span class="sxs-lookup"><span data-stu-id="c9356-166">principalName</span></span>| <span data-ttu-id="c9356-167">String</span><span class="sxs-lookup"><span data-stu-id="c9356-167">String</span></span> | <span data-ttu-id="c9356-168">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="c9356-168">Name of the principal.</span></span>|
|<span data-ttu-id="c9356-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="c9356-169">externalPrincipalId</span></span>| <span data-ttu-id="c9356-170">String</span><span class="sxs-lookup"><span data-stu-id="c9356-170">String</span></span> | <span data-ttu-id="c9356-171">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c9356-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="c9356-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="c9356-172">highestGrade</span></span>|<span data-ttu-id="c9356-173">String</span><span class="sxs-lookup"><span data-stu-id="c9356-173">String</span></span>| <span data-ttu-id="c9356-174">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="c9356-174">Highest grade taught.</span></span> |
|<span data-ttu-id="c9356-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="c9356-175">lowestGrade</span></span>|<span data-ttu-id="c9356-176">String</span><span class="sxs-lookup"><span data-stu-id="c9356-176">String</span></span>| <span data-ttu-id="c9356-177">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="c9356-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="c9356-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="c9356-178">schoolNumber</span></span>|<span data-ttu-id="c9356-179">String</span><span class="sxs-lookup"><span data-stu-id="c9356-179">String</span></span>| <span data-ttu-id="c9356-180">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-180">School Number.</span></span>|
|<span data-ttu-id="c9356-181">externalId</span><span class="sxs-lookup"><span data-stu-id="c9356-181">externalId</span></span>|<span data-ttu-id="c9356-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9356-182">String</span></span>| <span data-ttu-id="c9356-183">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c9356-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="c9356-184">phone</span><span class="sxs-lookup"><span data-stu-id="c9356-184">phone</span></span>|<span data-ttu-id="c9356-185">String</span><span class="sxs-lookup"><span data-stu-id="c9356-185">String</span></span>| <span data-ttu-id="c9356-186">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-186">Phone number of school.</span></span> |
|<span data-ttu-id="c9356-187">fax</span><span class="sxs-lookup"><span data-stu-id="c9356-187">fax</span></span>|<span data-ttu-id="c9356-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9356-188">String</span></span>| <span data-ttu-id="c9356-189">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-189">Fax number of school.</span></span> |
|<span data-ttu-id="c9356-190">address</span><span class="sxs-lookup"><span data-stu-id="c9356-190">address</span></span>|[<span data-ttu-id="c9356-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c9356-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="c9356-192">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-192">Address of the school.</span></span>|
|<span data-ttu-id="c9356-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="c9356-193">createdBy</span></span>|[<span data-ttu-id="c9356-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="c9356-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="c9356-195">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c9356-196">Relações</span><span class="sxs-lookup"><span data-stu-id="c9356-196">Relationships</span></span>
| <span data-ttu-id="c9356-197">Relação</span><span class="sxs-lookup"><span data-stu-id="c9356-197">Relationship</span></span> | <span data-ttu-id="c9356-198">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9356-198">Type</span></span>   |<span data-ttu-id="c9356-199">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9356-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9356-200">classes</span><span class="sxs-lookup"><span data-stu-id="c9356-200">classes</span></span>|<span data-ttu-id="c9356-201">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="c9356-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="c9356-202">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-202">Classes taught at the school.</span></span> <span data-ttu-id="c9356-203">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9356-203">Nullable.</span></span>|
|<span data-ttu-id="c9356-204">users</span><span class="sxs-lookup"><span data-stu-id="c9356-204">users</span></span>|<span data-ttu-id="c9356-205">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="c9356-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="c9356-206">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="c9356-206">Users in the school.</span></span> <span data-ttu-id="c9356-207">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9356-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9356-208">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9356-208">JSON representation</span></span>

<span data-ttu-id="c9356-209">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9356-209">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationschool.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
