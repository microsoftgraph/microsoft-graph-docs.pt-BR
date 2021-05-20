---
title: Tipo de recurso conditionalAccess
description: O **recurso conditionalaccess** é o ponto de entrada para o modelo de objeto Conditinal Access. Ele não contém propriedades usáveis.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3683965cda79f003cb5e548101272d869be902b8
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547350"
---
# <a name="conditionalaccess-resource-type"></a><span data-ttu-id="0f9ae-104">Tipo de recurso conditionalaccess</span><span class="sxs-lookup"><span data-stu-id="0f9ae-104">conditionalaccess resource type</span></span>

<span data-ttu-id="0f9ae-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f9ae-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f9ae-106">O **recurso conditionalAccess** é o ponto de entrada do modelo de objeto Conditional Access.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-106">The **conditionalAccess** resource is the entry point for the Conditional Access object model.</span></span> <span data-ttu-id="0f9ae-107">Ele não contém propriedades usáveis.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-107">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="0f9ae-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0f9ae-108">Methods</span></span>

| <span data-ttu-id="0f9ae-109">Método</span><span class="sxs-lookup"><span data-stu-id="0f9ae-109">Method</span></span>           | <span data-ttu-id="0f9ae-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0f9ae-110">Return Type</span></span>    |<span data-ttu-id="0f9ae-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f9ae-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f9ae-112">Criar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0f9ae-112">Create conditionalAccessPolicy</span></span>](../api/conditionalaccessroot-post-policies.md) |[<span data-ttu-id="0f9ae-113">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0f9ae-113">conditionalAccessPolicy</span></span>](conditionalaccesspolicy.md)| <span data-ttu-id="0f9ae-114">Crie um novo **conditionalAccessPolicy** postando na coleção conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-114">Create a new **conditionalAccessPolicy** by posting to the conditionalAccessPolicy collection.</span></span>|
|[<span data-ttu-id="0f9ae-115">Criar namedLocations</span><span class="sxs-lookup"><span data-stu-id="0f9ae-115">Create namedLocations</span></span>](../api/conditionalaccessroot-post-namedlocations.md) |[<span data-ttu-id="0f9ae-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="0f9ae-116">namedLocation</span></span>](namedlocation.md)| <span data-ttu-id="0f9ae-117">Crie um novo **namedLocations** postando na coleção namedLocations.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-117">Create a new **namedLocations** by posting to the namedLocations collection.</span></span>|
|[<span data-ttu-id="0f9ae-118">Criar authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="0f9ae-118">Create authenticationContextClassReferences</span></span>](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md)|[<span data-ttu-id="0f9ae-119">authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="0f9ae-119">authenticationContextClassReferences</span></span>](authenticationcontextclassreference.md)|<span data-ttu-id="0f9ae-120">Crie uma nova **autenticaçãoContextClassReferences** postando na coleção authenticationContextClassReferences.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-120">Create a new **authenticationContextClassReferences** by posting to authenticationContextClassReferences collection.</span></span>|


## <a name="properties"></a><span data-ttu-id="0f9ae-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f9ae-121">Properties</span></span>

<span data-ttu-id="0f9ae-122">O recurso conditionalAccess é o ponto de entrada para o modelo de objeto do Access Condicional e não contém nenhuma propriedade.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-122">The conditionalAccess resource is the entry point for the Conditional Access object model and doesn't contain any properties.</span></span>

## <a name="relationships"></a><span data-ttu-id="0f9ae-123">Relações</span><span class="sxs-lookup"><span data-stu-id="0f9ae-123">Relationships</span></span>
| <span data-ttu-id="0f9ae-124">Relação</span><span class="sxs-lookup"><span data-stu-id="0f9ae-124">Relationship</span></span> | <span data-ttu-id="0f9ae-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f9ae-125">Type</span></span>   |<span data-ttu-id="0f9ae-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f9ae-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f9ae-127">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0f9ae-127">conditionalAccessPolicy</span></span>|<span data-ttu-id="0f9ae-128">[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="0f9ae-128">[conditionalAccessPolicy](conditionalaccesspolicy.md) collection</span></span>| <span data-ttu-id="0f9ae-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-129">Read-only.</span></span> <span data-ttu-id="0f9ae-130">Anulável.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-130">Nullable.</span></span> <span data-ttu-id="0f9ae-131">Retorna uma coleção das políticas de Acesso Condicional especificadas.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-131">Returns a collection of the specified Conditional Access policies.</span></span>|
|<span data-ttu-id="0f9ae-132">namedLocations</span><span class="sxs-lookup"><span data-stu-id="0f9ae-132">namedLocations</span></span>|<span data-ttu-id="0f9ae-133">[Coleção namedLocations](namedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="0f9ae-133">[namedLocations](namedlocation.md) collection</span></span>| <span data-ttu-id="0f9ae-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-134">Read-only.</span></span> <span data-ttu-id="0f9ae-135">Anulável.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-135">Nullable.</span></span> <span data-ttu-id="0f9ae-136">Retorna uma coleção dos locais nomeados especificados.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-136">Returns a collection of the specified named locations.</span></span>|
|<span data-ttu-id="0f9ae-137">authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="0f9ae-137">authenticationContextClassReferences</span></span>|<span data-ttu-id="0f9ae-138">[Coleção authenticationContextClassReferences](authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="0f9ae-138">[authenticationContextClassReferences](authenticationcontextclassreference.md) collection</span></span>|<span data-ttu-id="0f9ae-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-139">Read-only.</span></span> <span data-ttu-id="0f9ae-140">Anulável.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-140">Nullable.</span></span> <span data-ttu-id="0f9ae-141">Retorna uma coleção das referências de classe de contexto de autenticação especificadas.</span><span class="sxs-lookup"><span data-stu-id="0f9ae-141">Returns a collection of the specified authentication context class references.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditional access resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

