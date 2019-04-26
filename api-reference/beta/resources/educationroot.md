---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 83879a2fe448e97f62dc592b42d1cbc1d3d5cf39
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334182"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="be7e4-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="be7e4-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be7e4-104">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="be7e4-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="be7e4-105">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="be7e4-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="be7e4-106">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="be7e4-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="be7e4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="be7e4-107">Methods</span></span>

| <span data-ttu-id="be7e4-108">Método</span><span class="sxs-lookup"><span data-stu-id="be7e4-108">Method</span></span>           | <span data-ttu-id="be7e4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="be7e4-109">Return Type</span></span>    |<span data-ttu-id="be7e4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="be7e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be7e4-111">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="be7e4-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="be7e4-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="be7e4-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="be7e4-113">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="be7e4-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="be7e4-114">Listar classes</span><span class="sxs-lookup"><span data-stu-id="be7e4-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="be7e4-115">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="be7e4-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="be7e4-116">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="be7e4-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="be7e4-117">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="be7e4-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="be7e4-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="be7e4-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="be7e4-119">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="be7e4-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="be7e4-120">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="be7e4-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="be7e4-121">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="be7e4-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="be7e4-122">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="be7e4-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="be7e4-123">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="be7e4-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="be7e4-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="be7e4-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="be7e4-125">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="be7e4-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="be7e4-126">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="be7e4-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="be7e4-127">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="be7e4-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="be7e4-128">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="be7e4-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="be7e4-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be7e4-129">Properties</span></span>
<span data-ttu-id="be7e4-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be7e4-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="be7e4-131">Relações</span><span class="sxs-lookup"><span data-stu-id="be7e4-131">Relationships</span></span>
| <span data-ttu-id="be7e4-132">Relação</span><span class="sxs-lookup"><span data-stu-id="be7e4-132">Relationship</span></span> | <span data-ttu-id="be7e4-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="be7e4-133">Type</span></span>   |<span data-ttu-id="be7e4-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="be7e4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be7e4-135">classes</span><span class="sxs-lookup"><span data-stu-id="be7e4-135">classes</span></span>|<span data-ttu-id="be7e4-136">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="be7e4-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="be7e4-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be7e4-137">Read-only.</span></span> <span data-ttu-id="be7e4-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="be7e4-138">Nullable.</span></span>|
|<span data-ttu-id="be7e4-139">me</span><span class="sxs-lookup"><span data-stu-id="be7e4-139">me</span></span>|[<span data-ttu-id="be7e4-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="be7e4-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="be7e4-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be7e4-141">Read-only.</span></span> <span data-ttu-id="be7e4-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="be7e4-142">Nullable.</span></span>|
|<span data-ttu-id="be7e4-143">schools</span><span class="sxs-lookup"><span data-stu-id="be7e4-143">schools</span></span>|<span data-ttu-id="be7e4-144">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="be7e4-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="be7e4-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be7e4-145">Read-only.</span></span> <span data-ttu-id="be7e4-146">Anulável.</span><span class="sxs-lookup"><span data-stu-id="be7e4-146">Nullable.</span></span>|
|<span data-ttu-id="be7e4-147">users</span><span class="sxs-lookup"><span data-stu-id="be7e4-147">users</span></span>|<span data-ttu-id="be7e4-148">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="be7e4-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="be7e4-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="be7e4-p105">Read-only. Nullable.</span></span>|

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
