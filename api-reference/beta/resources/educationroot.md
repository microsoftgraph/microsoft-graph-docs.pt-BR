---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 91f0162402b8c87042fab622710d314f27d6f4e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523509"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="c447c-103">Tipo de recurso educationRoot</span><span class="sxs-lookup"><span data-stu-id="c447c-103">educationRoot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c447c-104">O namespace `/education` expõe funcionalidade específica ao setor de educação.</span><span class="sxs-lookup"><span data-stu-id="c447c-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="c447c-105">Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)).</span><span class="sxs-lookup"><span data-stu-id="c447c-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="c447c-106">O namespace education fornece propriedades e recursos específicos de educação nesses objetos.</span><span class="sxs-lookup"><span data-stu-id="c447c-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="c447c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c447c-107">Methods</span></span>

| <span data-ttu-id="c447c-108">Método</span><span class="sxs-lookup"><span data-stu-id="c447c-108">Method</span></span>           | <span data-ttu-id="c447c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c447c-109">Return Type</span></span>    |<span data-ttu-id="c447c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c447c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c447c-111">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="c447c-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="c447c-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="c447c-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="c447c-113">Crie uma nova **educationClass** postando na coleção de aulas.</span><span class="sxs-lookup"><span data-stu-id="c447c-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="c447c-114">Listar classes</span><span class="sxs-lookup"><span data-stu-id="c447c-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="c447c-115">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="c447c-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="c447c-116">Obtenha uma coleção de objetos **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="c447c-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="c447c-117">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="c447c-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="c447c-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="c447c-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="c447c-119">Crie uma nova **educationSchool** postando na coleção de escolas.</span><span class="sxs-lookup"><span data-stu-id="c447c-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="c447c-120">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="c447c-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="c447c-121">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="c447c-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="c447c-122">Obtenha uma coleção de objetos **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="c447c-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="c447c-123">Criar educationUser</span><span class="sxs-lookup"><span data-stu-id="c447c-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="c447c-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="c447c-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c447c-125">Crie um novo **educationUser** postando na coleção de usuários.</span><span class="sxs-lookup"><span data-stu-id="c447c-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="c447c-126">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="c447c-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="c447c-127">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="c447c-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="c447c-128">Obtenha uma coleção de objetos **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="c447c-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="c447c-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c447c-129">Properties</span></span>
<span data-ttu-id="c447c-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c447c-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="c447c-131">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="c447c-131">Relationships</span></span>
| <span data-ttu-id="c447c-132">Relação</span><span class="sxs-lookup"><span data-stu-id="c447c-132">Relationship</span></span> | <span data-ttu-id="c447c-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c447c-133">Type</span></span>   |<span data-ttu-id="c447c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c447c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c447c-135">classes</span><span class="sxs-lookup"><span data-stu-id="c447c-135">classes</span></span>|<span data-ttu-id="c447c-136">Coleção [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="c447c-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="c447c-p102">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c447c-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="c447c-139">me</span><span class="sxs-lookup"><span data-stu-id="c447c-139">me</span></span>|[<span data-ttu-id="c447c-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="c447c-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="c447c-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c447c-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="c447c-143">schools</span><span class="sxs-lookup"><span data-stu-id="c447c-143">schools</span></span>|<span data-ttu-id="c447c-144">Coleção [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="c447c-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="c447c-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c447c-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="c447c-147">users</span><span class="sxs-lookup"><span data-stu-id="c447c-147">users</span></span>|<span data-ttu-id="c447c-148">Coleção [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="c447c-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="c447c-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c447c-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationroot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
