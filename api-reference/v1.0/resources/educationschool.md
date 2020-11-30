---
title: Tipo de recurso educationSchool
description: 'Recurso usado para gerenciar aulas, professores e alunos da escola representada.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: bd25283390e2683affe2e2cb636344c60a772a2e
ms.sourcegitcommit: 6714f71e0d229f1ab56150a9976b5106b4c8b785
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2020
ms.locfileid: "49368163"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="09769-103">Tipo de recurso educationSchool</span><span class="sxs-lookup"><span data-stu-id="09769-103">educationSchool resource type</span></span>

<span data-ttu-id="09769-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09769-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09769-105">Recurso usado para gerenciar aulas, professores e alunos da escola representada.</span><span class="sxs-lookup"><span data-stu-id="09769-105">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  

## <a name="methods"></a><span data-ttu-id="09769-106">Methods</span><span class="sxs-lookup"><span data-stu-id="09769-106">Methods</span></span>

| <span data-ttu-id="09769-107">Método</span><span class="sxs-lookup"><span data-stu-id="09769-107">Method</span></span>                                                   | <span data-ttu-id="09769-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="09769-108">Return Type</span></span>                                    | <span data-ttu-id="09769-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="09769-109">Description</span></span>                                                                                 |
| :------------------------------------------------------- | :--------------------------------------------- | :------------------------------------------------------------------------------------------ |
| [<span data-ttu-id="09769-110">Get</span><span class="sxs-lookup"><span data-stu-id="09769-110">Get</span></span>](../api/educationschool-get.md)                     | [<span data-ttu-id="09769-111">educationSchool</span><span class="sxs-lookup"><span data-stu-id="09769-111">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="09769-112">Leia as propriedades e relações de um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="09769-112">Read properties and relationships of an **educationSchool** object.</span></span>                         |
| [<span data-ttu-id="09769-113">Adicionar classe</span><span class="sxs-lookup"><span data-stu-id="09769-113">Add class</span></span>](../api/educationschool-post-classes.md)      | [<span data-ttu-id="09769-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="09769-114">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="09769-115">Adicione uma nova **educationClass** para a escola postando na propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="09769-115">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>  |
| [<span data-ttu-id="09769-116">Listar classes</span><span class="sxs-lookup"><span data-stu-id="09769-116">List classes</span></span>](../api/educationschool-list-classes.md)   | <span data-ttu-id="09769-117">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="09769-117">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="09769-118">Obtenha a coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="09769-118">Get the **educationClass** object collection.</span></span>                                               |
| [<span data-ttu-id="09769-119">Remover classe</span><span class="sxs-lookup"><span data-stu-id="09769-119">Remove class</span></span>](../api/educationschool-delete-classes.md) | [<span data-ttu-id="09769-120">educationClass</span><span class="sxs-lookup"><span data-stu-id="09769-120">educationClass</span></span>](educationclass.md)            | <span data-ttu-id="09769-121">Remova uma **educationClass** da escola por meio da propriedade de navegação de aulas.</span><span class="sxs-lookup"><span data-stu-id="09769-121">Remove an **educationClass** from the school through the classes navigation property.</span></span>       |
| [<span data-ttu-id="09769-122">Adicionar usuário</span><span class="sxs-lookup"><span data-stu-id="09769-122">Add user</span></span>](../api/educationschool-post-users.md)         | [<span data-ttu-id="09769-123">educationUser</span><span class="sxs-lookup"><span data-stu-id="09769-123">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="09769-124">Adicione um novo **educationUser** para a escola postando na propriedade de navegação de **usuários**.</span><span class="sxs-lookup"><span data-stu-id="09769-124">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span> |
| [<span data-ttu-id="09769-125">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="09769-125">List users</span></span>](../api/educationschool-list-users.md)       | <span data-ttu-id="09769-126">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="09769-126">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="09769-127">Obtenha a coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="09769-127">Get the **educationUser** object collection.</span></span>                                                |
| [<span data-ttu-id="09769-128">Remover usuário</span><span class="sxs-lookup"><span data-stu-id="09769-128">Remove user</span></span>](../api/educationschool-delete-users.md)    | [<span data-ttu-id="09769-129">educationUser</span><span class="sxs-lookup"><span data-stu-id="09769-129">educationUser</span></span>](educationuser.md)              | <span data-ttu-id="09769-130">Remova um **educationUser** da escola por meio da propriedade de navegação **users**.</span><span class="sxs-lookup"><span data-stu-id="09769-130">Remove an **educationUser** from the school through the **users** navigation property.</span></span>      |
| [<span data-ttu-id="09769-131">Atualizar</span><span class="sxs-lookup"><span data-stu-id="09769-131">Update</span></span>](../api/educationschool-update.md)               | [<span data-ttu-id="09769-132">educationSchool</span><span class="sxs-lookup"><span data-stu-id="09769-132">educationSchool</span></span>](educationschool.md)          | <span data-ttu-id="09769-133">Atualize um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="09769-133">Update an **educationSchool** object.</span></span>                                                       |
| [<span data-ttu-id="09769-134">Excluir</span><span class="sxs-lookup"><span data-stu-id="09769-134">Delete</span></span>](../api/educationschool-delete.md)               | <span data-ttu-id="09769-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09769-135">None</span></span>                                           | <span data-ttu-id="09769-136">Exclua um objeto **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="09769-136">Delete an **educationSchool** object.</span></span>                                                       |

## <a name="properties"></a><span data-ttu-id="09769-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09769-137">Properties</span></span>

| <span data-ttu-id="09769-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09769-138">Property</span></span>            | <span data-ttu-id="09769-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="09769-139">Type</span></span>                                  | <span data-ttu-id="09769-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="09769-140">Description</span></span>                                                                        |
| :------------------ | :------------------------------------ | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="09769-141">id</span><span class="sxs-lookup"><span data-stu-id="09769-141">id</span></span>                  | <span data-ttu-id="09769-142">String</span><span class="sxs-lookup"><span data-stu-id="09769-142">String</span></span>                                | <span data-ttu-id="09769-143">GUID desta escola.</span><span class="sxs-lookup"><span data-stu-id="09769-143">GUID of this school.</span></span>                                                               |
| <span data-ttu-id="09769-144">displayName</span><span class="sxs-lookup"><span data-stu-id="09769-144">displayName</span></span>         | <span data-ttu-id="09769-145">String</span><span class="sxs-lookup"><span data-stu-id="09769-145">String</span></span>                                | <span data-ttu-id="09769-146">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="09769-146">Display name of the school.</span></span>                                                        |
| <span data-ttu-id="09769-147">description</span><span class="sxs-lookup"><span data-stu-id="09769-147">description</span></span>         | <span data-ttu-id="09769-148">String</span><span class="sxs-lookup"><span data-stu-id="09769-148">String</span></span>                                | <span data-ttu-id="09769-149">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="09769-149">Description of the school.</span></span>                                                         |
| <span data-ttu-id="09769-150">status</span><span class="sxs-lookup"><span data-stu-id="09769-150">status</span></span>              | <span data-ttu-id="09769-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09769-151">string</span></span>                                | <span data-ttu-id="09769-152">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="09769-152">Read-Only.</span></span> <span data-ttu-id="09769-153">Os valores possíveis são: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="09769-153">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span> |
| <span data-ttu-id="09769-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="09769-154">externalSource</span></span>      | <span data-ttu-id="09769-155">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="09769-155">educationExternalSource</span></span>               | <span data-ttu-id="09769-156">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="09769-156">Read-Only.</span></span>  <span data-ttu-id="09769-157">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="09769-157">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>        |
| <span data-ttu-id="09769-158">principalEmail</span><span class="sxs-lookup"><span data-stu-id="09769-158">principalEmail</span></span>      | <span data-ttu-id="09769-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09769-159">String</span></span>                                | <span data-ttu-id="09769-160">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="09769-160">Email address of the principal.</span></span>                                                    |
| <span data-ttu-id="09769-161">principalName</span><span class="sxs-lookup"><span data-stu-id="09769-161">principalName</span></span>       | <span data-ttu-id="09769-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09769-162">String</span></span>                                | <span data-ttu-id="09769-163">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="09769-163">Name of the principal.</span></span>                                                             |
| <span data-ttu-id="09769-164">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="09769-164">externalPrincipalId</span></span> | <span data-ttu-id="09769-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09769-165">String</span></span>                                | <span data-ttu-id="09769-166">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="09769-166">ID of principal in syncing system.</span></span>                                                 |
| <span data-ttu-id="09769-167">highestGrade</span><span class="sxs-lookup"><span data-stu-id="09769-167">highestGrade</span></span>        | <span data-ttu-id="09769-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09769-168">String</span></span>                                | <span data-ttu-id="09769-169">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="09769-169">Highest grade taught.</span></span>                                                              |
| <span data-ttu-id="09769-170">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="09769-170">lowestGrade</span></span>         | <span data-ttu-id="09769-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09769-171">String</span></span>                                | <span data-ttu-id="09769-172">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="09769-172">Lowest grade taught.</span></span>                                                               |
| <span data-ttu-id="09769-173">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="09769-173">schoolNumber</span></span>        | <span data-ttu-id="09769-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09769-174">String</span></span>                                | <span data-ttu-id="09769-175">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="09769-175">School Number.</span></span>                                                                     |
| <span data-ttu-id="09769-176">externalId</span><span class="sxs-lookup"><span data-stu-id="09769-176">externalId</span></span>          | <span data-ttu-id="09769-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09769-177">String</span></span>                                | <span data-ttu-id="09769-178">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="09769-178">ID of school in syncing system.</span></span>                                                    |
| <span data-ttu-id="09769-179">phone</span><span class="sxs-lookup"><span data-stu-id="09769-179">phone</span></span>               | <span data-ttu-id="09769-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09769-180">String</span></span>                                | <span data-ttu-id="09769-181">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="09769-181">Phone number of school.</span></span>                                                            |
| <span data-ttu-id="09769-182">address</span><span class="sxs-lookup"><span data-stu-id="09769-182">address</span></span>             | [<span data-ttu-id="09769-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="09769-183">physicalAddress</span></span>](physicaladdress.md) | <span data-ttu-id="09769-184">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="09769-184">Address of the school.</span></span>                                                             |
| <span data-ttu-id="09769-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="09769-185">createdBy</span></span>           | [<span data-ttu-id="09769-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="09769-186">identitySet</span></span>](identityset.md)         | <span data-ttu-id="09769-187">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="09769-187">Entity who created the school.</span></span>                                                     |

## <a name="relationships"></a><span data-ttu-id="09769-188">Relações</span><span class="sxs-lookup"><span data-stu-id="09769-188">Relationships</span></span>

| <span data-ttu-id="09769-189">Relação</span><span class="sxs-lookup"><span data-stu-id="09769-189">Relationship</span></span> | <span data-ttu-id="09769-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="09769-190">Type</span></span>                                           | <span data-ttu-id="09769-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="09769-191">Description</span></span>                             |
| :----------- | :--------------------------------------------- | :-------------------------------------- |
| <span data-ttu-id="09769-192">classes</span><span class="sxs-lookup"><span data-stu-id="09769-192">classes</span></span>      | <span data-ttu-id="09769-193">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="09769-193">[educationClass](educationclass.md) collection</span></span> | <span data-ttu-id="09769-194">Aulas ministradas na escola.</span><span class="sxs-lookup"><span data-stu-id="09769-194">Classes taught at the school.</span></span> <span data-ttu-id="09769-195">Anulável.</span><span class="sxs-lookup"><span data-stu-id="09769-195">Nullable.</span></span> |
| <span data-ttu-id="09769-196">users</span><span class="sxs-lookup"><span data-stu-id="09769-196">users</span></span>        | <span data-ttu-id="09769-197">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="09769-197">[educationUser](educationuser.md) collection</span></span>   | <span data-ttu-id="09769-198">Usuários na escola.</span><span class="sxs-lookup"><span data-stu-id="09769-198">Users in the school.</span></span> <span data-ttu-id="09769-199">Anulável.</span><span class="sxs-lookup"><span data-stu-id="09769-199">Nullable.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="09769-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09769-200">JSON representation</span></span>

<span data-ttu-id="09769-201">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09769-201">The following is a JSON representation of the resource.</span></span>

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
  "phone": "String"
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

