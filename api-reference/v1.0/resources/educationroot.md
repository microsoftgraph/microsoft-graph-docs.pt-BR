---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3792f0c867538c77522566110be36ac15d952396
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531544"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="a889a-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="a889a-103">educationRoot resource type</span></span>

<span data-ttu-id="a889a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a889a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a889a-105">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="a889a-105">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="a889a-106">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="a889a-106">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="a889a-107">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="a889a-107">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="a889a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a889a-108">Methods</span></span>

| <span data-ttu-id="a889a-109">Método</span><span class="sxs-lookup"><span data-stu-id="a889a-109">Method</span></span>           | <span data-ttu-id="a889a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a889a-110">Return Type</span></span>    |<span data-ttu-id="a889a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a889a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a889a-112">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="a889a-112">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="a889a-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="a889a-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="a889a-114">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="a889a-114">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="a889a-115">Listar classes</span><span class="sxs-lookup"><span data-stu-id="a889a-115">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="a889a-116">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="a889a-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="a889a-117">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="a889a-117">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="a889a-118">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="a889a-118">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="a889a-119">educationSchool</span><span class="sxs-lookup"><span data-stu-id="a889a-119">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="a889a-120">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="a889a-120">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="a889a-121">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="a889a-121">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="a889a-122">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="a889a-122">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="a889a-123">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="a889a-123">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="a889a-124">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="a889a-124">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="a889a-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="a889a-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a889a-126">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="a889a-126">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="a889a-127">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="a889a-127">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="a889a-128">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="a889a-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="a889a-129">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="a889a-129">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a889a-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a889a-130">Properties</span></span>
<span data-ttu-id="a889a-131">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a889a-131">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="a889a-132">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="a889a-132">Relationships</span></span>
| <span data-ttu-id="a889a-133">Relação</span><span class="sxs-lookup"><span data-stu-id="a889a-133">Relationship</span></span> | <span data-ttu-id="a889a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a889a-134">Type</span></span>   |<span data-ttu-id="a889a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a889a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a889a-136">classes</span><span class="sxs-lookup"><span data-stu-id="a889a-136">classes</span></span>|<span data-ttu-id="a889a-137">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="a889a-137">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="a889a-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a889a-138">Read-only.</span></span> <span data-ttu-id="a889a-139">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a889a-139">Nullable.</span></span>|
|<span data-ttu-id="a889a-140">me</span><span class="sxs-lookup"><span data-stu-id="a889a-140">me</span></span>|[<span data-ttu-id="a889a-141">educationUser</span><span class="sxs-lookup"><span data-stu-id="a889a-141">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a889a-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a889a-142">Read-only.</span></span> <span data-ttu-id="a889a-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a889a-143">Nullable.</span></span>|
|<span data-ttu-id="a889a-144">schools</span><span class="sxs-lookup"><span data-stu-id="a889a-144">schools</span></span>|<span data-ttu-id="a889a-145">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="a889a-145">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="a889a-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="a889a-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="a889a-148">users</span><span class="sxs-lookup"><span data-stu-id="a889a-148">users</span></span>|<span data-ttu-id="a889a-149">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="a889a-149">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="a889a-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="a889a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a889a-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a889a-152">JSON representation</span></span>
<span data-ttu-id="a889a-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a889a-153">Here is a JSON representation of the resource.</span></span>

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


# <a name="http"></a>[<span data-ttu-id="a889a-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="a889a-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education
```
# <a name="c"></a>[<span data-ttu-id="a889a-155">C#</span><span class="sxs-lookup"><span data-stu-id="a889a-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a889a-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a889a-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a889a-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a889a-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a889a-158">Java</span><span class="sxs-lookup"><span data-stu-id="a889a-158">Java</span></span>](#tab/java)
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
