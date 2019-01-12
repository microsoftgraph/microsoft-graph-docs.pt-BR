---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e610ca79dcef29d85a9190c9d3d9429cbf3b363d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949651"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="d2dda-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="d2dda-103">educationRoot resource type</span></span>

> <span data-ttu-id="d2dda-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d2dda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2dda-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d2dda-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2dda-106">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="d2dda-106">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="d2dda-107">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="d2dda-107">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="d2dda-108">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="d2dda-108">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="d2dda-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2dda-109">Methods</span></span>

| <span data-ttu-id="d2dda-110">Método</span><span class="sxs-lookup"><span data-stu-id="d2dda-110">Method</span></span>           | <span data-ttu-id="d2dda-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d2dda-111">Return Type</span></span>    |<span data-ttu-id="d2dda-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2dda-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2dda-113">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="d2dda-113">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="d2dda-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="d2dda-114">educationClass</span></span>](educationclass.md)| <span data-ttu-id="d2dda-115">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="d2dda-115">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="d2dda-116">Listar classes</span><span class="sxs-lookup"><span data-stu-id="d2dda-116">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="d2dda-117">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="d2dda-117">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="d2dda-118">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="d2dda-118">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="d2dda-119">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="d2dda-119">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="d2dda-120">educationSchool</span><span class="sxs-lookup"><span data-stu-id="d2dda-120">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="d2dda-121">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="d2dda-121">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="d2dda-122">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="d2dda-122">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="d2dda-123">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="d2dda-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="d2dda-124">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="d2dda-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="d2dda-125">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="d2dda-125">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="d2dda-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="d2dda-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="d2dda-127">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="d2dda-127">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="d2dda-128">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="d2dda-128">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="d2dda-129">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="d2dda-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="d2dda-130">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="d2dda-130">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2dda-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2dda-131">Properties</span></span>
<span data-ttu-id="d2dda-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d2dda-132">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="d2dda-133">Relações</span><span class="sxs-lookup"><span data-stu-id="d2dda-133">Relationships</span></span>
| <span data-ttu-id="d2dda-134">Relação</span><span class="sxs-lookup"><span data-stu-id="d2dda-134">Relationship</span></span> | <span data-ttu-id="d2dda-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2dda-135">Type</span></span>   |<span data-ttu-id="d2dda-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2dda-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2dda-137">classes</span><span class="sxs-lookup"><span data-stu-id="d2dda-137">classes</span></span>|<span data-ttu-id="d2dda-138">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="d2dda-138">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="d2dda-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d2dda-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="d2dda-141">me</span><span class="sxs-lookup"><span data-stu-id="d2dda-141">me</span></span>|[<span data-ttu-id="d2dda-142">educationUser</span><span class="sxs-lookup"><span data-stu-id="d2dda-142">educationUser</span></span>](educationuser.md)| <span data-ttu-id="d2dda-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d2dda-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="d2dda-145">schools</span><span class="sxs-lookup"><span data-stu-id="d2dda-145">schools</span></span>|<span data-ttu-id="d2dda-146">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="d2dda-146">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="d2dda-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d2dda-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="d2dda-149">users</span><span class="sxs-lookup"><span data-stu-id="d2dda-149">users</span></span>|<span data-ttu-id="d2dda-150">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="d2dda-150">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="d2dda-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d2dda-p106">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
