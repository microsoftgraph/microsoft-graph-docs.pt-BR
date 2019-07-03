---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 84b7312515174c19837a5cda3fa3ffb466f65c23
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458751"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="e7dc0-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="e7dc0-103">educationRoot resource type</span></span>

<span data-ttu-id="e7dc0-104">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="e7dc0-105">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="e7dc0-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="e7dc0-106">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="e7dc0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e7dc0-107">Methods</span></span>

| <span data-ttu-id="e7dc0-108">Método</span><span class="sxs-lookup"><span data-stu-id="e7dc0-108">Method</span></span>           | <span data-ttu-id="e7dc0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e7dc0-109">Return Type</span></span>    |<span data-ttu-id="e7dc0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7dc0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7dc0-111">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="e7dc0-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="e7dc0-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="e7dc0-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="e7dc0-113">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="e7dc0-114">Listar classes</span><span class="sxs-lookup"><span data-stu-id="e7dc0-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="e7dc0-115">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="e7dc0-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="e7dc0-116">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="e7dc0-117">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="e7dc0-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="e7dc0-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="e7dc0-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="e7dc0-119">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="e7dc0-120">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="e7dc0-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="e7dc0-121">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="e7dc0-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="e7dc0-122">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="e7dc0-123">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="e7dc0-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="e7dc0-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="e7dc0-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e7dc0-125">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="e7dc0-126">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="e7dc0-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="e7dc0-127">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="e7dc0-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e7dc0-128">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="e7dc0-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7dc0-129">Properties</span></span>
<span data-ttu-id="e7dc0-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e7dc0-131">Relações</span><span class="sxs-lookup"><span data-stu-id="e7dc0-131">Relationships</span></span>
| <span data-ttu-id="e7dc0-132">Relação</span><span class="sxs-lookup"><span data-stu-id="e7dc0-132">Relationship</span></span> | <span data-ttu-id="e7dc0-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7dc0-133">Type</span></span>   |<span data-ttu-id="e7dc0-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7dc0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7dc0-135">classes</span><span class="sxs-lookup"><span data-stu-id="e7dc0-135">classes</span></span>|<span data-ttu-id="e7dc0-136">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="e7dc0-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="e7dc0-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-137">Read-only.</span></span> <span data-ttu-id="e7dc0-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-138">Nullable.</span></span>|
|<span data-ttu-id="e7dc0-139">me</span><span class="sxs-lookup"><span data-stu-id="e7dc0-139">me</span></span>|[<span data-ttu-id="e7dc0-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="e7dc0-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e7dc0-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-141">Read-only.</span></span> <span data-ttu-id="e7dc0-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-142">Nullable.</span></span>|
|<span data-ttu-id="e7dc0-143">schools</span><span class="sxs-lookup"><span data-stu-id="e7dc0-143">schools</span></span>|<span data-ttu-id="e7dc0-144">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="e7dc0-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="e7dc0-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="e7dc0-147">users</span><span class="sxs-lookup"><span data-stu-id="e7dc0-147">users</span></span>|<span data-ttu-id="e7dc0-148">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="e7dc0-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e7dc0-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7dc0-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7dc0-151">JSON representation</span></span>
<span data-ttu-id="e7dc0-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7dc0-152">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```


# <a name="httptabhttp"></a>[<span data-ttu-id="e7dc0-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7dc0-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7dc0-154">C#</span><span class="sxs-lookup"><span data-stu-id="e7dc0-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7dc0-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7dc0-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7dc0-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e7dc0-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
