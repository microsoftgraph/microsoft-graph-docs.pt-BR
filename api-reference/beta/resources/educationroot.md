---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: c268c7b910bd9f6f14763f3a7b5445af0ac12826
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890654"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="8908f-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="8908f-103">educationRoot resource type</span></span>

> <span data-ttu-id="8908f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8908f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8908f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8908f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8908f-106">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="8908f-106">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="8908f-107">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="8908f-107">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="8908f-108">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="8908f-108">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="8908f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="8908f-109">Methods</span></span>

| <span data-ttu-id="8908f-110">Método</span><span class="sxs-lookup"><span data-stu-id="8908f-110">Method</span></span>           | <span data-ttu-id="8908f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8908f-111">Return Type</span></span>    |<span data-ttu-id="8908f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8908f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8908f-113">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="8908f-113">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="8908f-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="8908f-114">educationClass</span></span>](educationclass.md)| <span data-ttu-id="8908f-115">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="8908f-115">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="8908f-116">Listar classes</span><span class="sxs-lookup"><span data-stu-id="8908f-116">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="8908f-117">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="8908f-117">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="8908f-118">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="8908f-118">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="8908f-119">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="8908f-119">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="8908f-120">educationSchool</span><span class="sxs-lookup"><span data-stu-id="8908f-120">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="8908f-121">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="8908f-121">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="8908f-122">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="8908f-122">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="8908f-123">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="8908f-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="8908f-124">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="8908f-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="8908f-125">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="8908f-125">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="8908f-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="8908f-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8908f-127">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="8908f-127">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="8908f-128">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="8908f-128">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="8908f-129">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="8908f-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="8908f-130">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="8908f-130">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="8908f-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8908f-131">Properties</span></span>
<span data-ttu-id="8908f-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8908f-132">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="8908f-133">Relações</span><span class="sxs-lookup"><span data-stu-id="8908f-133">Relationships</span></span>
| <span data-ttu-id="8908f-134">Relação</span><span class="sxs-lookup"><span data-stu-id="8908f-134">Relationship</span></span> | <span data-ttu-id="8908f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="8908f-135">Type</span></span>   |<span data-ttu-id="8908f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="8908f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8908f-137">classes</span><span class="sxs-lookup"><span data-stu-id="8908f-137">classes</span></span>|<span data-ttu-id="8908f-138">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="8908f-138">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="8908f-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8908f-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8908f-141">me</span><span class="sxs-lookup"><span data-stu-id="8908f-141">me</span></span>|[<span data-ttu-id="8908f-142">educationUser</span><span class="sxs-lookup"><span data-stu-id="8908f-142">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8908f-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8908f-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8908f-145">schools</span><span class="sxs-lookup"><span data-stu-id="8908f-145">schools</span></span>|<span data-ttu-id="8908f-146">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="8908f-146">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="8908f-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8908f-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8908f-149">users</span><span class="sxs-lookup"><span data-stu-id="8908f-149">users</span></span>|<span data-ttu-id="8908f-150">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="8908f-150">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="8908f-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8908f-p106">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
