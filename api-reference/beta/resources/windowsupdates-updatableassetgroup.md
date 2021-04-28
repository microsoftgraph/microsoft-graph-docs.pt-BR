---
title: Tipo de recurso updatableAssetGroup
description: Um grupo de recursos do azureADDevice que podem receber atualizações.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a3aca42b69a906f167393cfd284d6756b3c4bb52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067233"
---
# <a name="updatableassetgroup-resource-type"></a><span data-ttu-id="b5e07-103">Tipo de recurso updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="b5e07-103">updatableAssetGroup resource type</span></span>

<span data-ttu-id="b5e07-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="b5e07-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5e07-105">Um grupo de [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) que podem receber atualizações.</span><span class="sxs-lookup"><span data-stu-id="b5e07-105">A group of [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources that can receive updates.</span></span>

<span data-ttu-id="b5e07-106">Os membros são do tipo de [recurso azureADDevice.](../resources/windowsupdates-azureADDevice.md)</span><span class="sxs-lookup"><span data-stu-id="b5e07-106">Members are of the [azureADDevice](../resources/windowsupdates-azureADDevice.md) resource type.</span></span> <span data-ttu-id="b5e07-107">Um **recurso updatableAssetGroup** não pode ser membro de outro **updatableAssetGroup**.</span><span class="sxs-lookup"><span data-stu-id="b5e07-107">An **updatableAssetGroup** resource cannot be a member of another **updatableAssetGroup**.</span></span>

<span data-ttu-id="b5e07-108">Herda de [updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="b5e07-108">Inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b5e07-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="b5e07-109">Methods</span></span>
|<span data-ttu-id="b5e07-110">Método</span><span class="sxs-lookup"><span data-stu-id="b5e07-110">Method</span></span>|<span data-ttu-id="b5e07-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b5e07-111">Return type</span></span>|<span data-ttu-id="b5e07-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5e07-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b5e07-113">Listar recursos updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="b5e07-113">List updatableAssetGroup resources</span></span>](../api/windowsupdates-updates-list-updatableassets-updatableassetgroup.md)|<span data-ttu-id="b5e07-114">[coleção microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b5e07-114">[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) collection</span></span>|<span data-ttu-id="b5e07-115">Obter uma lista dos objetos [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b5e07-115">Get a list of the [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects and their properties.</span></span>|
|[<span data-ttu-id="b5e07-116">Criar updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="b5e07-116">Create updatableAssetGroup</span></span>](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[<span data-ttu-id="b5e07-117">microsoft.graph.windowsUpdates.updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="b5e07-117">microsoft.graph.windowsUpdates.updatableAssetGroup</span></span>](../resources/windowsupdates-updatableassetgroup.md)|<span data-ttu-id="b5e07-118">Crie um novo [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b5e07-118">Create a new [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="b5e07-119">Obter updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="b5e07-119">Get updatableAssetGroup</span></span>](../api/windowsupdates-updatableassetgroup-get.md)|[<span data-ttu-id="b5e07-120">microsoft.graph.windowsUpdates.updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="b5e07-120">microsoft.graph.windowsUpdates.updatableAssetGroup</span></span>](../resources/windowsupdates-updatableassetgroup.md)|<span data-ttu-id="b5e07-121">Leia as propriedades e as relações de um [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b5e07-121">Read the properties and relationships of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="b5e07-122">Excluir updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="b5e07-122">Delete updatableAssetGroup</span></span>](../api/windowsupdates-updatableassetgroup-delete.md)|<span data-ttu-id="b5e07-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5e07-123">None</span></span>|<span data-ttu-id="b5e07-124">Exclui um [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b5e07-124">Deletes an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="b5e07-125">Adicionar membros</span><span class="sxs-lookup"><span data-stu-id="b5e07-125">Add members</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)|<span data-ttu-id="b5e07-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5e07-126">None</span></span>|<span data-ttu-id="b5e07-127">Adicionar membros a [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="b5e07-127">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="b5e07-128">Adicionar membros (por ID)</span><span class="sxs-lookup"><span data-stu-id="b5e07-128">Add members (by ID)</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)|<span data-ttu-id="b5e07-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5e07-129">None</span></span>|<span data-ttu-id="b5e07-130">Adicionar membros a [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="b5e07-130">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="b5e07-131">Remover membros</span><span class="sxs-lookup"><span data-stu-id="b5e07-131">Remove members</span></span>](../api/windowsupdates-updatableassetgroup-removemembers.md)|<span data-ttu-id="b5e07-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5e07-132">None</span></span>|<span data-ttu-id="b5e07-133">Remover membros de [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="b5e07-133">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="b5e07-134">Remover membros (por ID)</span><span class="sxs-lookup"><span data-stu-id="b5e07-134">Remove members (by ID)</span></span>](../api/windowsupdates-updatableassetgroup-removemembers.md)|<span data-ttu-id="b5e07-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5e07-135">None</span></span>|<span data-ttu-id="b5e07-136">Remover membros de [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="b5e07-136">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="b5e07-137">Listar membros</span><span class="sxs-lookup"><span data-stu-id="b5e07-137">List members</span></span>](../api/windowsupdates-updatableassetgroup-list-members.md)|<span data-ttu-id="b5e07-138">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b5e07-138">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b5e07-139">Obter os [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) da propriedade de navegação membros.</span><span class="sxs-lookup"><span data-stu-id="b5e07-139">Get the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources from the members navigation property.</span></span>|

## <a name="properties"></a><span data-ttu-id="b5e07-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5e07-140">Properties</span></span>
|<span data-ttu-id="b5e07-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5e07-141">Property</span></span>|<span data-ttu-id="b5e07-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5e07-142">Type</span></span>|<span data-ttu-id="b5e07-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5e07-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5e07-144">id</span><span class="sxs-lookup"><span data-stu-id="b5e07-144">id</span></span>|<span data-ttu-id="b5e07-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5e07-145">String</span></span>|<span data-ttu-id="b5e07-146">Um identificador para o grupo.</span><span class="sxs-lookup"><span data-stu-id="b5e07-146">An identifier for the group.</span></span> <span data-ttu-id="b5e07-147">Chave.</span><span class="sxs-lookup"><span data-stu-id="b5e07-147">Key.</span></span> <span data-ttu-id="b5e07-148">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="b5e07-148">Not nullable.</span></span> <span data-ttu-id="b5e07-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5e07-149">Read-only.</span></span> <span data-ttu-id="b5e07-150">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="b5e07-150">Returned by default.</span></span> <span data-ttu-id="b5e07-151">Herdado [de updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="b5e07-151">Inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5e07-152">Relações</span><span class="sxs-lookup"><span data-stu-id="b5e07-152">Relationships</span></span>
|<span data-ttu-id="b5e07-153">Relação</span><span class="sxs-lookup"><span data-stu-id="b5e07-153">Relationship</span></span>|<span data-ttu-id="b5e07-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5e07-154">Type</span></span>|<span data-ttu-id="b5e07-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5e07-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5e07-156">membros</span><span class="sxs-lookup"><span data-stu-id="b5e07-156">members</span></span>|<span data-ttu-id="b5e07-157">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b5e07-157">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b5e07-158">Membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="b5e07-158">Members of the group.</span></span> <span data-ttu-id="b5e07-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5e07-159">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5e07-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5e07-160">JSON representation</span></span>
<span data-ttu-id="b5e07-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5e07-161">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "String (identifier)"
}
```

