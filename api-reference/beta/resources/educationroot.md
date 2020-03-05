---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 14e152fa5aa24366eade56b632d96e2c4e4bfcc8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501056"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="06515-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="06515-103">educationRoot resource type</span></span>

<span data-ttu-id="06515-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06515-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06515-105">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="06515-105">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="06515-106">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="06515-106">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="06515-107">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="06515-107">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="06515-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="06515-108">Methods</span></span>

| <span data-ttu-id="06515-109">Método</span><span class="sxs-lookup"><span data-stu-id="06515-109">Method</span></span>           | <span data-ttu-id="06515-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="06515-110">Return Type</span></span>    |<span data-ttu-id="06515-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="06515-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06515-112">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="06515-112">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="06515-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="06515-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="06515-114">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="06515-114">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="06515-115">Listar classes</span><span class="sxs-lookup"><span data-stu-id="06515-115">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="06515-116">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="06515-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="06515-117">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="06515-117">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="06515-118">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="06515-118">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="06515-119">educationSchool</span><span class="sxs-lookup"><span data-stu-id="06515-119">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="06515-120">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="06515-120">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="06515-121">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="06515-121">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="06515-122">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="06515-122">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="06515-123">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="06515-123">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="06515-124">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="06515-124">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="06515-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="06515-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="06515-126">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="06515-126">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="06515-127">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="06515-127">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="06515-128">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="06515-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="06515-129">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="06515-129">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="06515-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06515-130">Properties</span></span>
<span data-ttu-id="06515-131">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="06515-131">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="06515-132">Relações</span><span class="sxs-lookup"><span data-stu-id="06515-132">Relationships</span></span>
| <span data-ttu-id="06515-133">Relação</span><span class="sxs-lookup"><span data-stu-id="06515-133">Relationship</span></span> | <span data-ttu-id="06515-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="06515-134">Type</span></span>   |<span data-ttu-id="06515-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="06515-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06515-136">classes</span><span class="sxs-lookup"><span data-stu-id="06515-136">classes</span></span>|<span data-ttu-id="06515-137">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="06515-137">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="06515-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="06515-138">Read-only.</span></span> <span data-ttu-id="06515-139">Anulável.</span><span class="sxs-lookup"><span data-stu-id="06515-139">Nullable.</span></span>|
|<span data-ttu-id="06515-140">me</span><span class="sxs-lookup"><span data-stu-id="06515-140">me</span></span>|[<span data-ttu-id="06515-141">educationUser</span><span class="sxs-lookup"><span data-stu-id="06515-141">educationUser</span></span>](educationuser.md)| <span data-ttu-id="06515-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="06515-142">Read-only.</span></span> <span data-ttu-id="06515-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="06515-143">Nullable.</span></span>|
|<span data-ttu-id="06515-144">schools</span><span class="sxs-lookup"><span data-stu-id="06515-144">schools</span></span>|<span data-ttu-id="06515-145">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="06515-145">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="06515-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="06515-146">Read-only.</span></span> <span data-ttu-id="06515-147">Anulável.</span><span class="sxs-lookup"><span data-stu-id="06515-147">Nullable.</span></span>|
|<span data-ttu-id="06515-148">users</span><span class="sxs-lookup"><span data-stu-id="06515-148">users</span></span>|<span data-ttu-id="06515-149">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="06515-149">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="06515-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="06515-p105">Read-only. Nullable.</span></span>|

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
