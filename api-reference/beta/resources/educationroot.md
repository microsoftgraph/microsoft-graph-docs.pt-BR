---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8084b1aae61ffb9e9982fbf8b5f4b8e430a85da1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972562"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="bb238-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="bb238-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb238-104">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="bb238-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="bb238-105">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="bb238-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="bb238-106">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="bb238-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="bb238-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="bb238-107">Methods</span></span>

| <span data-ttu-id="bb238-108">Método</span><span class="sxs-lookup"><span data-stu-id="bb238-108">Method</span></span>           | <span data-ttu-id="bb238-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bb238-109">Return Type</span></span>    |<span data-ttu-id="bb238-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb238-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb238-111">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="bb238-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="bb238-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="bb238-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="bb238-113">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="bb238-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="bb238-114">Listar classes</span><span class="sxs-lookup"><span data-stu-id="bb238-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="bb238-115">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="bb238-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="bb238-116">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="bb238-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="bb238-117">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="bb238-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="bb238-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="bb238-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="bb238-119">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="bb238-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="bb238-120">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="bb238-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="bb238-121">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="bb238-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="bb238-122">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="bb238-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="bb238-123">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="bb238-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="bb238-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="bb238-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="bb238-125">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="bb238-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="bb238-126">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="bb238-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="bb238-127">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="bb238-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="bb238-128">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="bb238-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb238-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb238-129">Properties</span></span>
<span data-ttu-id="bb238-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bb238-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="bb238-131">Relações</span><span class="sxs-lookup"><span data-stu-id="bb238-131">Relationships</span></span>
| <span data-ttu-id="bb238-132">Relação</span><span class="sxs-lookup"><span data-stu-id="bb238-132">Relationship</span></span> | <span data-ttu-id="bb238-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb238-133">Type</span></span>   |<span data-ttu-id="bb238-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb238-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb238-135">classes</span><span class="sxs-lookup"><span data-stu-id="bb238-135">classes</span></span>|<span data-ttu-id="bb238-136">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="bb238-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="bb238-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb238-137">Read-only.</span></span> <span data-ttu-id="bb238-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bb238-138">Nullable.</span></span>|
|<span data-ttu-id="bb238-139">me</span><span class="sxs-lookup"><span data-stu-id="bb238-139">me</span></span>|[<span data-ttu-id="bb238-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="bb238-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="bb238-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb238-141">Read-only.</span></span> <span data-ttu-id="bb238-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bb238-142">Nullable.</span></span>|
|<span data-ttu-id="bb238-143">schools</span><span class="sxs-lookup"><span data-stu-id="bb238-143">schools</span></span>|<span data-ttu-id="bb238-144">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="bb238-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="bb238-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb238-145">Read-only.</span></span> <span data-ttu-id="bb238-146">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bb238-146">Nullable.</span></span>|
|<span data-ttu-id="bb238-147">users</span><span class="sxs-lookup"><span data-stu-id="bb238-147">users</span></span>|<span data-ttu-id="bb238-148">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="bb238-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="bb238-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="bb238-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
