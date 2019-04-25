---
title: Tipo de recurso educationSchool
description: 'Uma escola. O recurso **educationSchool** atualmente corresponde a um recurso administrativeUnit e compartilha a mesma ID.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542911"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="4816c-104">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="4816c-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4816c-105">Uma escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-105">A school.</span></span> <span data-ttu-id="4816c-106">O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="4816c-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="4816c-107">Esse recurso é um subtipo de [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="4816c-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="4816c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="4816c-108">Methods</span></span>

| <span data-ttu-id="4816c-109">Método</span><span class="sxs-lookup"><span data-stu-id="4816c-109">Method</span></span>           | <span data-ttu-id="4816c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4816c-110">Return Type</span></span>    |<span data-ttu-id="4816c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4816c-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4816c-112">Obter</span><span class="sxs-lookup"><span data-stu-id="4816c-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="4816c-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="4816c-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="4816c-114">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="4816c-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="4816c-115">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="4816c-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="4816c-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="4816c-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="4816c-117">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="4816c-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="4816c-118">Listar classes</span><span class="sxs-lookup"><span data-stu-id="4816c-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="4816c-119">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="4816c-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="4816c-120">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="4816c-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="4816c-121">Remover classe</span><span class="sxs-lookup"><span data-stu-id="4816c-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="4816c-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="4816c-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="4816c-123">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="4816c-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="4816c-124">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="4816c-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="4816c-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="4816c-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="4816c-126">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="4816c-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="4816c-127">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="4816c-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="4816c-128">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="4816c-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="4816c-129">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="4816c-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="4816c-130">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="4816c-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="4816c-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="4816c-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="4816c-132">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="4816c-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="4816c-133">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="4816c-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="4816c-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="4816c-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="4816c-135">Obtenha o **administrativeUnit** que corresponde a esse **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="4816c-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="4816c-136">Atualizar</span><span class="sxs-lookup"><span data-stu-id="4816c-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="4816c-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="4816c-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="4816c-138">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="4816c-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="4816c-139">Excluir</span><span class="sxs-lookup"><span data-stu-id="4816c-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="4816c-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4816c-140">None</span></span> |<span data-ttu-id="4816c-141">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="4816c-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4816c-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4816c-142">Properties</span></span>
| <span data-ttu-id="4816c-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4816c-143">Property</span></span>     | <span data-ttu-id="4816c-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="4816c-144">Type</span></span>   |<span data-ttu-id="4816c-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="4816c-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4816c-146">id</span><span class="sxs-lookup"><span data-stu-id="4816c-146">id</span></span>|<span data-ttu-id="4816c-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4816c-147">String</span></span>|<span data-ttu-id="4816c-148">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-148">GUID of this school.</span></span>|
|<span data-ttu-id="4816c-149">displayName</span><span class="sxs-lookup"><span data-stu-id="4816c-149">displayName</span></span>| <span data-ttu-id="4816c-150">String</span><span class="sxs-lookup"><span data-stu-id="4816c-150">String</span></span>| <span data-ttu-id="4816c-151">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-151">Display name of the school.</span></span>| 
|<span data-ttu-id="4816c-152">description</span><span class="sxs-lookup"><span data-stu-id="4816c-152">description</span></span>| <span data-ttu-id="4816c-153">String</span><span class="sxs-lookup"><span data-stu-id="4816c-153">String</span></span> | <span data-ttu-id="4816c-154">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-154">Description of the school.</span></span>| 
|<span data-ttu-id="4816c-155">status</span><span class="sxs-lookup"><span data-stu-id="4816c-155">status</span></span>| <span data-ttu-id="4816c-156">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4816c-156">string</span></span>| <span data-ttu-id="4816c-157">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="4816c-157">Read-Only.</span></span> <span data-ttu-id="4816c-158">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="4816c-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="4816c-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="4816c-159">externalSource</span></span>| <span data-ttu-id="4816c-160">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4816c-160">string</span></span>| <span data-ttu-id="4816c-161">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="4816c-161">Read-Only.</span></span>  <span data-ttu-id="4816c-162">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4816c-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4816c-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="4816c-163">principalEmail</span></span>| <span data-ttu-id="4816c-164">String</span><span class="sxs-lookup"><span data-stu-id="4816c-164">String</span></span>| <span data-ttu-id="4816c-165">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="4816c-165">Email address of the principal.</span></span>|
|<span data-ttu-id="4816c-166">principalName</span><span class="sxs-lookup"><span data-stu-id="4816c-166">principalName</span></span>| <span data-ttu-id="4816c-167">String</span><span class="sxs-lookup"><span data-stu-id="4816c-167">String</span></span> | <span data-ttu-id="4816c-168">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="4816c-168">Name of the principal.</span></span>|
|<span data-ttu-id="4816c-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="4816c-169">externalPrincipalId</span></span>| <span data-ttu-id="4816c-170">String</span><span class="sxs-lookup"><span data-stu-id="4816c-170">String</span></span> | <span data-ttu-id="4816c-171">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4816c-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="4816c-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="4816c-172">highestGrade</span></span>|<span data-ttu-id="4816c-173">String</span><span class="sxs-lookup"><span data-stu-id="4816c-173">String</span></span>| <span data-ttu-id="4816c-174">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="4816c-174">Highest grade taught.</span></span> |
|<span data-ttu-id="4816c-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="4816c-175">lowestGrade</span></span>|<span data-ttu-id="4816c-176">String</span><span class="sxs-lookup"><span data-stu-id="4816c-176">String</span></span>| <span data-ttu-id="4816c-177">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="4816c-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="4816c-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="4816c-178">schoolNumber</span></span>|<span data-ttu-id="4816c-179">String</span><span class="sxs-lookup"><span data-stu-id="4816c-179">String</span></span>| <span data-ttu-id="4816c-180">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-180">School Number.</span></span>|
|<span data-ttu-id="4816c-181">externalId</span><span class="sxs-lookup"><span data-stu-id="4816c-181">externalId</span></span>|<span data-ttu-id="4816c-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4816c-182">String</span></span>| <span data-ttu-id="4816c-183">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4816c-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="4816c-184">phone</span><span class="sxs-lookup"><span data-stu-id="4816c-184">phone</span></span>|<span data-ttu-id="4816c-185">String</span><span class="sxs-lookup"><span data-stu-id="4816c-185">String</span></span>| <span data-ttu-id="4816c-186">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-186">Phone number of school.</span></span> |
|<span data-ttu-id="4816c-187">fax</span><span class="sxs-lookup"><span data-stu-id="4816c-187">fax</span></span>|<span data-ttu-id="4816c-188">String</span><span class="sxs-lookup"><span data-stu-id="4816c-188">String</span></span>| <span data-ttu-id="4816c-189">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-189">Fax number of school.</span></span> |
|<span data-ttu-id="4816c-190">address</span><span class="sxs-lookup"><span data-stu-id="4816c-190">address</span></span>|[<span data-ttu-id="4816c-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4816c-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="4816c-192">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-192">Address of the school.</span></span>|
|<span data-ttu-id="4816c-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="4816c-193">createdBy</span></span>|[<span data-ttu-id="4816c-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="4816c-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="4816c-195">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4816c-196">Relações</span><span class="sxs-lookup"><span data-stu-id="4816c-196">Relationships</span></span>
| <span data-ttu-id="4816c-197">Relação</span><span class="sxs-lookup"><span data-stu-id="4816c-197">Relationship</span></span> | <span data-ttu-id="4816c-198">Tipo</span><span class="sxs-lookup"><span data-stu-id="4816c-198">Type</span></span>   |<span data-ttu-id="4816c-199">Descrição</span><span class="sxs-lookup"><span data-stu-id="4816c-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4816c-200">classes</span><span class="sxs-lookup"><span data-stu-id="4816c-200">classes</span></span>|<span data-ttu-id="4816c-201">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="4816c-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="4816c-202">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-202">Classes taught at the school.</span></span> <span data-ttu-id="4816c-203">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4816c-203">Nullable.</span></span>|
|<span data-ttu-id="4816c-204">users</span><span class="sxs-lookup"><span data-stu-id="4816c-204">users</span></span>|<span data-ttu-id="4816c-205">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="4816c-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="4816c-206">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="4816c-206">Users in the school.</span></span> <span data-ttu-id="4816c-207">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4816c-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4816c-208">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4816c-208">JSON representation</span></span>

<span data-ttu-id="4816c-209">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4816c-209">The following is a JSON representation of the resource.</span></span>

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
