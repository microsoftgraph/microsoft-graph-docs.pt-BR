---
title: Tipo de recurso educationSchool
description: 'Escola A. O recurso **educationSchool** atualmente corresponde a um recurso administrativeUnit e compartilha a mesma ID.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 17a5c3ad2f28e802bb6cad3a97d1cb723b3407d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918242"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="7d53d-104">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="7d53d-104">educationSchool resource type</span></span>

> <span data-ttu-id="7d53d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d53d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d53d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d53d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d53d-107">Escola A.</span><span class="sxs-lookup"><span data-stu-id="7d53d-107">A school.</span></span> <span data-ttu-id="7d53d-108">O recurso **educationSchool** atualmente corresponde a um recurso [administrativeUnit](administrativeunit.md) e compartilha a mesma ID.</span><span class="sxs-lookup"><span data-stu-id="7d53d-108">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="7d53d-109">Esse recurso é um subtipo de [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="7d53d-109">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="7d53d-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d53d-110">Methods</span></span>

| <span data-ttu-id="7d53d-111">Método</span><span class="sxs-lookup"><span data-stu-id="7d53d-111">Method</span></span>           | <span data-ttu-id="7d53d-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d53d-112">Return Type</span></span>    |<span data-ttu-id="7d53d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d53d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d53d-114">Obter</span><span class="sxs-lookup"><span data-stu-id="7d53d-114">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="7d53d-115">educationSchool</span><span class="sxs-lookup"><span data-stu-id="7d53d-115">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="7d53d-116">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="7d53d-116">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="7d53d-117">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="7d53d-117">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="7d53d-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="7d53d-118">educationClass</span></span>](educationclass.md)| <span data-ttu-id="7d53d-119">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="7d53d-119">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="7d53d-120">Listar classes</span><span class="sxs-lookup"><span data-stu-id="7d53d-120">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="7d53d-121">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="7d53d-121">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="7d53d-122">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="7d53d-122">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="7d53d-123">Remover classe</span><span class="sxs-lookup"><span data-stu-id="7d53d-123">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="7d53d-124">educationClass</span><span class="sxs-lookup"><span data-stu-id="7d53d-124">educationClass</span></span>](educationclass.md)| <span data-ttu-id="7d53d-125">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="7d53d-125">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="7d53d-126">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="7d53d-126">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="7d53d-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="7d53d-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="7d53d-128">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="7d53d-128">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="7d53d-129">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="7d53d-129">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="7d53d-130">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="7d53d-130">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="7d53d-131">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="7d53d-131">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="7d53d-132">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="7d53d-132">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="7d53d-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="7d53d-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="7d53d-134">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="7d53d-134">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="7d53d-135">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="7d53d-135">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="7d53d-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="7d53d-136">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="7d53d-137">Obtenha a **administrativeUnit** que corresponde a essa **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="7d53d-137">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="7d53d-138">Atualizar</span><span class="sxs-lookup"><span data-stu-id="7d53d-138">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="7d53d-139">educationSchool</span><span class="sxs-lookup"><span data-stu-id="7d53d-139">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="7d53d-140">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="7d53d-140">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="7d53d-141">Excluir</span><span class="sxs-lookup"><span data-stu-id="7d53d-141">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="7d53d-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d53d-142">None</span></span> |<span data-ttu-id="7d53d-143">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="7d53d-143">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7d53d-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d53d-144">Properties</span></span>
| <span data-ttu-id="7d53d-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d53d-145">Property</span></span>     | <span data-ttu-id="7d53d-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d53d-146">Type</span></span>   |<span data-ttu-id="7d53d-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d53d-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d53d-148">id</span><span class="sxs-lookup"><span data-stu-id="7d53d-148">id</span></span>|<span data-ttu-id="7d53d-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-149">String</span></span>|<span data-ttu-id="7d53d-150">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-150">GUID of this school.</span></span>|
|<span data-ttu-id="7d53d-151">displayName</span><span class="sxs-lookup"><span data-stu-id="7d53d-151">displayName</span></span>| <span data-ttu-id="7d53d-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-152">String</span></span>| <span data-ttu-id="7d53d-153">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-153">Display name of the school.</span></span>| 
|<span data-ttu-id="7d53d-154">description</span><span class="sxs-lookup"><span data-stu-id="7d53d-154">description</span></span>| <span data-ttu-id="7d53d-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-155">String</span></span> | <span data-ttu-id="7d53d-156">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-156">Description of the school.</span></span>| 
|<span data-ttu-id="7d53d-157">status</span><span class="sxs-lookup"><span data-stu-id="7d53d-157">status</span></span>| <span data-ttu-id="7d53d-158">string</span><span class="sxs-lookup"><span data-stu-id="7d53d-158">string</span></span>| <span data-ttu-id="7d53d-159">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="7d53d-159">Read-Only.</span></span> <span data-ttu-id="7d53d-160">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="7d53d-160">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="7d53d-161">externalSource</span><span class="sxs-lookup"><span data-stu-id="7d53d-161">externalSource</span></span>| <span data-ttu-id="7d53d-162">string</span><span class="sxs-lookup"><span data-stu-id="7d53d-162">string</span></span>| <span data-ttu-id="7d53d-163">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="7d53d-163">Read-Only.</span></span>  <span data-ttu-id="7d53d-164">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="7d53d-164">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7d53d-165">principalEmail</span><span class="sxs-lookup"><span data-stu-id="7d53d-165">principalEmail</span></span>| <span data-ttu-id="7d53d-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-166">String</span></span>| <span data-ttu-id="7d53d-167">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="7d53d-167">Email address of the principal.</span></span>|
|<span data-ttu-id="7d53d-168">principalName</span><span class="sxs-lookup"><span data-stu-id="7d53d-168">principalName</span></span>| <span data-ttu-id="7d53d-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-169">String</span></span> | <span data-ttu-id="7d53d-170">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="7d53d-170">Name of the principal.</span></span>|
|<span data-ttu-id="7d53d-171">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="7d53d-171">externalPrincipalId</span></span>| <span data-ttu-id="7d53d-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-172">String</span></span> | <span data-ttu-id="7d53d-173">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7d53d-173">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="7d53d-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="7d53d-174">highestGrade</span></span>|<span data-ttu-id="7d53d-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-175">String</span></span>| <span data-ttu-id="7d53d-176">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="7d53d-176">Highest grade taught.</span></span> |
|<span data-ttu-id="7d53d-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="7d53d-177">lowestGrade</span></span>|<span data-ttu-id="7d53d-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-178">String</span></span>| <span data-ttu-id="7d53d-179">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="7d53d-179">Lowest grade taught.</span></span> |
|<span data-ttu-id="7d53d-180">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="7d53d-180">schoolNumber</span></span>|<span data-ttu-id="7d53d-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-181">String</span></span>| <span data-ttu-id="7d53d-182">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-182">School Number.</span></span>|
|<span data-ttu-id="7d53d-183">externalId</span><span class="sxs-lookup"><span data-stu-id="7d53d-183">externalId</span></span>|<span data-ttu-id="7d53d-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-184">String</span></span>| <span data-ttu-id="7d53d-185">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7d53d-185">ID of school in syncing system.</span></span> |
|<span data-ttu-id="7d53d-186">phone</span><span class="sxs-lookup"><span data-stu-id="7d53d-186">phone</span></span>|<span data-ttu-id="7d53d-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-187">String</span></span>| <span data-ttu-id="7d53d-188">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-188">Phone number of school.</span></span> |
|<span data-ttu-id="7d53d-189">fax</span><span class="sxs-lookup"><span data-stu-id="7d53d-189">fax</span></span>|<span data-ttu-id="7d53d-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d53d-190">String</span></span>| <span data-ttu-id="7d53d-191">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-191">Fax number of school.</span></span> |
|<span data-ttu-id="7d53d-192">address</span><span class="sxs-lookup"><span data-stu-id="7d53d-192">address</span></span>|[<span data-ttu-id="7d53d-193">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="7d53d-193">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="7d53d-194">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-194">Address of the school.</span></span>|
|<span data-ttu-id="7d53d-195">createdBy</span><span class="sxs-lookup"><span data-stu-id="7d53d-195">createdBy</span></span>|[<span data-ttu-id="7d53d-196">identitySet</span><span class="sxs-lookup"><span data-stu-id="7d53d-196">identitySet</span></span>](identityset.md)|<span data-ttu-id="7d53d-197">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-197">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7d53d-198">Relações</span><span class="sxs-lookup"><span data-stu-id="7d53d-198">Relationships</span></span>
| <span data-ttu-id="7d53d-199">Relação</span><span class="sxs-lookup"><span data-stu-id="7d53d-199">Relationship</span></span> | <span data-ttu-id="7d53d-200">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d53d-200">Type</span></span>   |<span data-ttu-id="7d53d-201">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d53d-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d53d-202">classes</span><span class="sxs-lookup"><span data-stu-id="7d53d-202">classes</span></span>|<span data-ttu-id="7d53d-203">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="7d53d-203">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="7d53d-204">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-204">Classes taught at the school.</span></span> <span data-ttu-id="7d53d-205">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7d53d-205">Nullable.</span></span>|
|<span data-ttu-id="7d53d-206">users</span><span class="sxs-lookup"><span data-stu-id="7d53d-206">users</span></span>|<span data-ttu-id="7d53d-207">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="7d53d-207">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="7d53d-208">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="7d53d-208">Users in the school.</span></span> <span data-ttu-id="7d53d-209">Anulável.</span><span class="sxs-lookup"><span data-stu-id="7d53d-209">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d53d-210">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d53d-210">JSON representation</span></span>

<span data-ttu-id="7d53d-211">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d53d-211">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
