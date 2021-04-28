---
title: Tipo de recurso deploymentAudience
description: O conjunto de recursos updatableAsset aos quais uma implantação pode ser aplicada.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 98d295183f69012da6ea9fc5803bc440465854c8
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067246"
---
# <a name="deploymentaudience-resource-type"></a><span data-ttu-id="ee18a-103">Tipo de recurso deploymentAudience</span><span class="sxs-lookup"><span data-stu-id="ee18a-103">deploymentAudience resource type</span></span>

<span data-ttu-id="ee18a-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ee18a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee18a-105">O conjunto de [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) aos quais uma [implantação](../resources/windowsupdates-deployment.md) pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="ee18a-105">The set of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to which a [deployment](../resources/windowsupdates-deployment.md) can apply.</span></span>

<span data-ttu-id="ee18a-106">Se o mesmo **recurso updatableAsset** estiver  incluído nas exclusões e relações de membros, a implantação não se aplicará a ele. </span><span class="sxs-lookup"><span data-stu-id="ee18a-106">If the same **updatableAsset** resource is included in the **exclusions** and **members** relationships, deployment will not apply to it.</span></span>

## <a name="methods"></a><span data-ttu-id="ee18a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ee18a-107">Methods</span></span>
|<span data-ttu-id="ee18a-108">Método</span><span class="sxs-lookup"><span data-stu-id="ee18a-108">Method</span></span>|<span data-ttu-id="ee18a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ee18a-109">Return type</span></span>|<span data-ttu-id="ee18a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee18a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee18a-111">Listar membros</span><span class="sxs-lookup"><span data-stu-id="ee18a-111">List members</span></span>](../api/windowsupdates-deploymentaudience-list-members.md)|<span data-ttu-id="ee18a-112">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="ee18a-112">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="ee18a-113">Listar membros da [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="ee18a-113">List members of the [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>|
|[<span data-ttu-id="ee18a-114">Exclusões de lista</span><span class="sxs-lookup"><span data-stu-id="ee18a-114">List exclusions</span></span>](../api/windowsupdates-deploymentaudience-list-exclusions.md)|<span data-ttu-id="ee18a-115">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="ee18a-115">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="ee18a-116">Listar exclusões da [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="ee18a-116">List exclusions of the [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>|
|[<span data-ttu-id="ee18a-117">Atualizar membros e exclusões</span><span class="sxs-lookup"><span data-stu-id="ee18a-117">Update members and exclusions</span></span>](../api/windowsupdates-deploymentaudience-updateaudience.md)|<span data-ttu-id="ee18a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee18a-118">None</span></span>|<span data-ttu-id="ee18a-119">Adicionar ou remover membros e exclusões.</span><span class="sxs-lookup"><span data-stu-id="ee18a-119">Add or remove members and exclusions.</span></span>|
|[<span data-ttu-id="ee18a-120">Atualizar membros e exclusões (por ID)</span><span class="sxs-lookup"><span data-stu-id="ee18a-120">Update members and exclusions (by ID)</span></span>](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)|<span data-ttu-id="ee18a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee18a-121">None</span></span>|<span data-ttu-id="ee18a-122">Adicione ou remova membros e exclusões do mesmo tipo.</span><span class="sxs-lookup"><span data-stu-id="ee18a-122">Add or remove members and exclusions of the same type.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee18a-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee18a-123">Properties</span></span>
|<span data-ttu-id="ee18a-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee18a-124">Property</span></span>|<span data-ttu-id="ee18a-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee18a-125">Type</span></span>|<span data-ttu-id="ee18a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee18a-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee18a-127">id</span><span class="sxs-lookup"><span data-stu-id="ee18a-127">id</span></span>|<span data-ttu-id="ee18a-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee18a-128">String</span></span>|<span data-ttu-id="ee18a-129">O identificador exclusivo para o público de implantação.</span><span class="sxs-lookup"><span data-stu-id="ee18a-129">The unique identifier for the deployment audience.</span></span> <span data-ttu-id="ee18a-130">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="ee18a-130">Returned by default.</span></span> <span data-ttu-id="ee18a-131">Chave.</span><span class="sxs-lookup"><span data-stu-id="ee18a-131">Key.</span></span> <span data-ttu-id="ee18a-132">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="ee18a-132">Not nullable.</span></span> <span data-ttu-id="ee18a-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee18a-133">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee18a-134">Relações</span><span class="sxs-lookup"><span data-stu-id="ee18a-134">Relationships</span></span>
|<span data-ttu-id="ee18a-135">Relação</span><span class="sxs-lookup"><span data-stu-id="ee18a-135">Relationship</span></span>|<span data-ttu-id="ee18a-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee18a-136">Type</span></span>|<span data-ttu-id="ee18a-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee18a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee18a-138">exclusões</span><span class="sxs-lookup"><span data-stu-id="ee18a-138">exclusions</span></span>|<span data-ttu-id="ee18a-139">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="ee18a-139">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="ee18a-140">Especifica os ativos a ser excluídos da audiência.</span><span class="sxs-lookup"><span data-stu-id="ee18a-140">Specifies the assets to exclude from the audience.</span></span>|
|<span data-ttu-id="ee18a-141">membros</span><span class="sxs-lookup"><span data-stu-id="ee18a-141">members</span></span>|<span data-ttu-id="ee18a-142">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="ee18a-142">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="ee18a-143">Especifica os ativos a ser incluídos na audiência.</span><span class="sxs-lookup"><span data-stu-id="ee18a-143">Specifies the assets to include in the audience.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee18a-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee18a-144">JSON representation</span></span>
<span data-ttu-id="ee18a-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee18a-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentAudience",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentAudience",
  "id": "String (identifier)"
}
```

