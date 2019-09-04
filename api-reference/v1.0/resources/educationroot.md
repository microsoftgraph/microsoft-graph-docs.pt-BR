---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 00afa9e91d350fedd023646ab952db641addb9f7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730348"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="87797-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="87797-103">educationRoot resource type</span></span>

<span data-ttu-id="87797-104">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="87797-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="87797-105">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="87797-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="87797-106">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="87797-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="87797-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="87797-107">Methods</span></span>

| <span data-ttu-id="87797-108">Método</span><span class="sxs-lookup"><span data-stu-id="87797-108">Method</span></span>           | <span data-ttu-id="87797-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="87797-109">Return Type</span></span>    |<span data-ttu-id="87797-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="87797-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="87797-111">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="87797-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="87797-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="87797-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="87797-113">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="87797-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="87797-114">Listar classes</span><span class="sxs-lookup"><span data-stu-id="87797-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="87797-115">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="87797-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="87797-116">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="87797-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="87797-117">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="87797-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="87797-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="87797-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="87797-119">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="87797-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="87797-120">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="87797-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="87797-121">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="87797-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="87797-122">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="87797-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="87797-123">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="87797-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="87797-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="87797-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="87797-125">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="87797-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="87797-126">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="87797-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="87797-127">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="87797-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="87797-128">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="87797-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="87797-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87797-129">Properties</span></span>
<span data-ttu-id="87797-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="87797-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="87797-131">Relações</span><span class="sxs-lookup"><span data-stu-id="87797-131">Relationships</span></span>
| <span data-ttu-id="87797-132">Relação</span><span class="sxs-lookup"><span data-stu-id="87797-132">Relationship</span></span> | <span data-ttu-id="87797-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="87797-133">Type</span></span>   |<span data-ttu-id="87797-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="87797-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87797-135">classes</span><span class="sxs-lookup"><span data-stu-id="87797-135">classes</span></span>|<span data-ttu-id="87797-136">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="87797-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="87797-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87797-137">Read-only.</span></span> <span data-ttu-id="87797-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="87797-138">Nullable.</span></span>|
|<span data-ttu-id="87797-139">me</span><span class="sxs-lookup"><span data-stu-id="87797-139">me</span></span>|[<span data-ttu-id="87797-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="87797-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="87797-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87797-141">Read-only.</span></span> <span data-ttu-id="87797-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="87797-142">Nullable.</span></span>|
|<span data-ttu-id="87797-143">schools</span><span class="sxs-lookup"><span data-stu-id="87797-143">schools</span></span>|<span data-ttu-id="87797-144">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="87797-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="87797-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="87797-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="87797-147">users</span><span class="sxs-lookup"><span data-stu-id="87797-147">users</span></span>|<span data-ttu-id="87797-148">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="87797-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="87797-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="87797-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87797-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87797-151">JSON representation</span></span>
<span data-ttu-id="87797-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87797-152">Here is a JSON representation of the resource.</span></span>

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


# <a name="httptabhttp"></a>[<span data-ttu-id="87797-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="87797-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="87797-154">C#</span><span class="sxs-lookup"><span data-stu-id="87797-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87797-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87797-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87797-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="87797-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="87797-157">Java</span><span class="sxs-lookup"><span data-stu-id="87797-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-education-java-snippets.md)]
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
