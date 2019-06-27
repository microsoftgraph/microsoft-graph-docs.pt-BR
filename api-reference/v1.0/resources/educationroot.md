---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 69835ca7e3c7a45864382eab9d1b362034873a60
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277907"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="3cb76-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="3cb76-103">educationRoot resource type</span></span>

<span data-ttu-id="3cb76-104">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="3cb76-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="3cb76-105">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="3cb76-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="3cb76-106">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="3cb76-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="3cb76-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3cb76-107">Methods</span></span>

| <span data-ttu-id="3cb76-108">Método</span><span class="sxs-lookup"><span data-stu-id="3cb76-108">Method</span></span>           | <span data-ttu-id="3cb76-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3cb76-109">Return Type</span></span>    |<span data-ttu-id="3cb76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cb76-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3cb76-111">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="3cb76-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="3cb76-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="3cb76-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="3cb76-113">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="3cb76-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="3cb76-114">Listar classes</span><span class="sxs-lookup"><span data-stu-id="3cb76-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="3cb76-115">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="3cb76-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="3cb76-116">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="3cb76-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="3cb76-117">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="3cb76-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="3cb76-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="3cb76-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="3cb76-119">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="3cb76-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="3cb76-120">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="3cb76-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="3cb76-121">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="3cb76-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="3cb76-122">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="3cb76-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="3cb76-123">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="3cb76-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="3cb76-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="3cb76-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="3cb76-125">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="3cb76-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="3cb76-126">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="3cb76-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="3cb76-127">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="3cb76-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="3cb76-128">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="3cb76-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="3cb76-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cb76-129">Properties</span></span>
<span data-ttu-id="3cb76-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3cb76-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="3cb76-131">Relações</span><span class="sxs-lookup"><span data-stu-id="3cb76-131">Relationships</span></span>
| <span data-ttu-id="3cb76-132">Relação</span><span class="sxs-lookup"><span data-stu-id="3cb76-132">Relationship</span></span> | <span data-ttu-id="3cb76-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cb76-133">Type</span></span>   |<span data-ttu-id="3cb76-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cb76-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cb76-135">classes</span><span class="sxs-lookup"><span data-stu-id="3cb76-135">classes</span></span>|<span data-ttu-id="3cb76-136">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="3cb76-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="3cb76-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3cb76-137">Read-only.</span></span> <span data-ttu-id="3cb76-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3cb76-138">Nullable.</span></span>|
|<span data-ttu-id="3cb76-139">me</span><span class="sxs-lookup"><span data-stu-id="3cb76-139">me</span></span>|[<span data-ttu-id="3cb76-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="3cb76-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="3cb76-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3cb76-141">Read-only.</span></span> <span data-ttu-id="3cb76-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3cb76-142">Nullable.</span></span>|
|<span data-ttu-id="3cb76-143">schools</span><span class="sxs-lookup"><span data-stu-id="3cb76-143">schools</span></span>|<span data-ttu-id="3cb76-144">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="3cb76-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="3cb76-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3cb76-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="3cb76-147">users</span><span class="sxs-lookup"><span data-stu-id="3cb76-147">users</span></span>|<span data-ttu-id="3cb76-148">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="3cb76-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="3cb76-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3cb76-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cb76-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cb76-151">JSON representation</span></span>
<span data-ttu-id="3cb76-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3cb76-152">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3cb76-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3cb76-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3cb76-154">C#</span><span class="sxs-lookup"><span data-stu-id="3cb76-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_education-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cb76-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cb76-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_education-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3cb76-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3cb76-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_education-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/educationroot.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
