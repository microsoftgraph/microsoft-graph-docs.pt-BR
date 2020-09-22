---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2ed10fd9be0a49fbf25acac635cf29b1759c31eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032653"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="61390-103">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="61390-103">educationSchool resource type</span></span>

<span data-ttu-id="61390-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61390-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61390-105">Recurso usado para gerenciar aulas, professores e alunos da escola representada.</span><span class="sxs-lookup"><span data-stu-id="61390-105">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="61390-106">Methods</span><span class="sxs-lookup"><span data-stu-id="61390-106">Methods</span></span>

| <span data-ttu-id="61390-107">Método</span><span class="sxs-lookup"><span data-stu-id="61390-107">Method</span></span>                                                   | <span data-ttu-id="61390-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="61390-108">Return Type</span></span>                                    | <span data-ttu-id="61390-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="61390-109">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="61390-110">Get</span><span class="sxs-lookup"><span data-stu-id="61390-110">Get</span></span>](../api/educationschool-get.md)                     | [<span data-ttu-id="61390-111">educationSchool</span><span class="sxs-lookup"><span data-stu-id="61390-111">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="61390-112">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="61390-112">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="61390-113">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="61390-113">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="61390-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="61390-114">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="61390-115">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="61390-115">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="61390-116">Listar classes</span><span class="sxs-lookup"><span data-stu-id="61390-116">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="61390-117">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="61390-117">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="61390-118">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="61390-118">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="61390-119">Remover classe</span><span class="sxs-lookup"><span data-stu-id="61390-119">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="61390-120">educationClass</span><span class="sxs-lookup"><span data-stu-id="61390-120">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="61390-121">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="61390-121">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="61390-122">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="61390-122">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="61390-123">educationUser</span><span class="sxs-lookup"><span data-stu-id="61390-123">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="61390-124">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="61390-124">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="61390-125">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="61390-125">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="61390-126">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="61390-126">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="61390-127">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="61390-127">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="61390-128">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="61390-128">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="61390-129">educationUser</span><span class="sxs-lookup"><span data-stu-id="61390-129">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="61390-130">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="61390-130">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="61390-131">Atualizar</span><span class="sxs-lookup"><span data-stu-id="61390-131">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="61390-132">educationSchool</span><span class="sxs-lookup"><span data-stu-id="61390-132">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="61390-133">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="61390-133">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="61390-134">Delete</span><span class="sxs-lookup"><span data-stu-id="61390-134">Delete</span></span>](../api/educationschool-delete.md)               | <span data-ttu-id="61390-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61390-135">None</span></span>                                           | <span data-ttu-id="61390-136">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="61390-136">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="61390-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61390-137">Properties</span></span>

| <span data-ttu-id="61390-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61390-138">Property</span></span>            | <span data-ttu-id="61390-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="61390-139">Type</span></span>                                  | <span data-ttu-id="61390-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="61390-140">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="61390-141">id</span><span class="sxs-lookup"><span data-stu-id="61390-141">id</span></span>                  | <span data-ttu-id="61390-142">String</span><span class="sxs-lookup"><span data-stu-id="61390-142">String</span></span>                                | <span data-ttu-id="61390-143">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="61390-143">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="61390-144">displayName</span><span class="sxs-lookup"><span data-stu-id="61390-144">displayName</span></span>         | <span data-ttu-id="61390-145">String</span><span class="sxs-lookup"><span data-stu-id="61390-145">String</span></span>                                | <span data-ttu-id="61390-146">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="61390-146">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="61390-147">description</span><span class="sxs-lookup"><span data-stu-id="61390-147">description</span></span>         | <span data-ttu-id="61390-148">String</span><span class="sxs-lookup"><span data-stu-id="61390-148">String</span></span>                                | <span data-ttu-id="61390-149">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="61390-149">Description of the school.</span></span>                                                         |
| <span data-ttu-id="61390-150">status</span><span class="sxs-lookup"><span data-stu-id="61390-150">status</span></span>              | <span data-ttu-id="61390-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61390-151">string</span></span>                                | <span data-ttu-id="61390-152">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="61390-152">Read-Only.</span></span> <span data-ttu-id="61390-153">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="61390-153">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="61390-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="61390-154">externalSource</span></span>      | <span data-ttu-id="61390-155">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="61390-155">educationExternalSource</span></span>               | <span data-ttu-id="61390-156">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="61390-156">Read-Only.</span></span>  <span data-ttu-id="61390-157">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="61390-157">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="61390-158">principalEmail</span><span class="sxs-lookup"><span data-stu-id="61390-158">principalEmail</span></span>      | <span data-ttu-id="61390-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61390-159">String</span></span>                                | <span data-ttu-id="61390-160">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="61390-160">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="61390-161">principalName</span><span class="sxs-lookup"><span data-stu-id="61390-161">principalName</span></span>       | <span data-ttu-id="61390-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61390-162">String</span></span>                                | <span data-ttu-id="61390-163">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="61390-163">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="61390-164">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="61390-164">externalPrincipalId</span></span> | <span data-ttu-id="61390-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61390-165">String</span></span>                                | <span data-ttu-id="61390-166">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="61390-166">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="61390-167">highestGrade</span><span class="sxs-lookup"><span data-stu-id="61390-167">highestGrade</span></span>        | <span data-ttu-id="61390-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61390-168">String</span></span>                                | <span data-ttu-id="61390-169">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="61390-169">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="61390-170">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="61390-170">lowestGrade</span></span>         | <span data-ttu-id="61390-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61390-171">String</span></span>                                | <span data-ttu-id="61390-172">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="61390-172">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="61390-173">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="61390-173">schoolNumber</span></span>        | <span data-ttu-id="61390-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61390-174">String</span></span>                                | <span data-ttu-id="61390-175">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="61390-175">School Number.</span></span>                                                                     |
| <span data-ttu-id="61390-176">externalId</span><span class="sxs-lookup"><span data-stu-id="61390-176">externalId</span></span>          | <span data-ttu-id="61390-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61390-177">String</span></span>                                | <span data-ttu-id="61390-178">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="61390-178">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="61390-179">phone</span><span class="sxs-lookup"><span data-stu-id="61390-179">phone</span></span>               | <span data-ttu-id="61390-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61390-180">String</span></span>                                | <span data-ttu-id="61390-181">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="61390-181">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="61390-182">address</span><span class="sxs-lookup"><span data-stu-id="61390-182">address</span></span>             | [<span data-ttu-id="61390-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="61390-183">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="61390-184">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="61390-184">Address of the school.</span></span>                                                             |
| <span data-ttu-id="61390-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="61390-185">createdBy</span></span>           | [<span data-ttu-id="61390-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="61390-186">identitySet</span></span>](identityset.md)         | <span data-ttu-id="61390-187">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="61390-187">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="61390-188">Relações</span><span class="sxs-lookup"><span data-stu-id="61390-188">Relationships</span></span>

| <span data-ttu-id="61390-189">Relação</span><span class="sxs-lookup"><span data-stu-id="61390-189">Relationship</span></span> | <span data-ttu-id="61390-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="61390-190">Type</span></span>                                           | <span data-ttu-id="61390-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="61390-191">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="61390-192">classes</span><span class="sxs-lookup"><span data-stu-id="61390-192">classes</span></span>      | <span data-ttu-id="61390-193">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="61390-193">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="61390-194">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="61390-194">Classes taught at the school.</span></span> <span data-ttu-id="61390-195">Anulável.</span><span class="sxs-lookup"><span data-stu-id="61390-195">Nullable.</span></span> |
| <span data-ttu-id="61390-196">users</span><span class="sxs-lookup"><span data-stu-id="61390-196">users</span></span>        | <span data-ttu-id="61390-197">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="61390-197">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="61390-198">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="61390-198">Users in the school.</span></span> <span data-ttu-id="61390-199">Anulável.</span><span class="sxs-lookup"><span data-stu-id="61390-199">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="61390-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61390-200">JSON representation</span></span>

<span data-ttu-id="61390-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61390-201">The following is a JSON representation of the resource.</span></span>

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

