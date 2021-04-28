---
title: tipo de recurso de implantação
description: Representa a implantação de conteúdo para um conjunto de dispositivos.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: e34bca8fc1776c749e42e97caa1dd0d91fa51433
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067797"
---
# <a name="deployment-resource-type"></a><span data-ttu-id="027d0-103">tipo de recurso de implantação</span><span class="sxs-lookup"><span data-stu-id="027d0-103">deployment resource type</span></span>

<span data-ttu-id="027d0-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="027d0-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="027d0-105">Representa a implantação de conteúdo para um conjunto de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="027d0-105">Represents the deployment of content to a set of devices.</span></span>

## <a name="methods"></a><span data-ttu-id="027d0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="027d0-106">Methods</span></span>
|<span data-ttu-id="027d0-107">Método</span><span class="sxs-lookup"><span data-stu-id="027d0-107">Method</span></span>|<span data-ttu-id="027d0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="027d0-108">Return type</span></span>|<span data-ttu-id="027d0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="027d0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="027d0-110">Listar implantações</span><span class="sxs-lookup"><span data-stu-id="027d0-110">List deployments</span></span>](../api/windowsupdates-updates-list-deployments.md)|<span data-ttu-id="027d0-111">[coleção microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="027d0-111">[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) collection</span></span>|<span data-ttu-id="027d0-112">Obter uma lista dos objetos [de implantação](../resources/windowsupdates-deployment.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="027d0-112">Get a list of the [deployment](../resources/windowsupdates-deployment.md) objects and their properties.</span></span>|
|[<span data-ttu-id="027d0-113">Criar implantação</span><span class="sxs-lookup"><span data-stu-id="027d0-113">Create deployment</span></span>](../api/windowsupdates-updates-post-deployments.md)|[<span data-ttu-id="027d0-114">microsoft.graph.windowsUpdates.deployment</span><span class="sxs-lookup"><span data-stu-id="027d0-114">microsoft.graph.windowsUpdates.deployment</span></span>](../resources/windowsupdates-deployment.md)|<span data-ttu-id="027d0-115">Crie um novo [objeto de implantação.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="027d0-115">Create a new [deployment](../resources/windowsupdates-deployment.md) object.</span></span>|
|[<span data-ttu-id="027d0-116">Obter implantação</span><span class="sxs-lookup"><span data-stu-id="027d0-116">Get deployment</span></span>](../api/windowsupdates-deployment-get.md)|[<span data-ttu-id="027d0-117">microsoft.graph.windowsUpdates.deployment</span><span class="sxs-lookup"><span data-stu-id="027d0-117">microsoft.graph.windowsUpdates.deployment</span></span>](../resources/windowsupdates-deployment.md)|<span data-ttu-id="027d0-118">Leia as propriedades e as relações de um [objeto de](../resources/windowsupdates-deployment.md) implantação.</span><span class="sxs-lookup"><span data-stu-id="027d0-118">Read the properties and relationships of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>|
|[<span data-ttu-id="027d0-119">Atualizar implantação</span><span class="sxs-lookup"><span data-stu-id="027d0-119">Update deployment</span></span>](../api/windowsupdates-deployment-update.md)|[<span data-ttu-id="027d0-120">microsoft.graph.windowsUpdates.deployment</span><span class="sxs-lookup"><span data-stu-id="027d0-120">microsoft.graph.windowsUpdates.deployment</span></span>](../resources/windowsupdates-deployment.md)|<span data-ttu-id="027d0-121">Atualize as propriedades de um [objeto de](../resources/windowsupdates-deployment.md) implantação.</span><span class="sxs-lookup"><span data-stu-id="027d0-121">Update the properties of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>|
|[<span data-ttu-id="027d0-122">Excluir implantação</span><span class="sxs-lookup"><span data-stu-id="027d0-122">Delete deployment</span></span>](../api/windowsupdates-deployment-delete.md)|<span data-ttu-id="027d0-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="027d0-123">None</span></span>|<span data-ttu-id="027d0-124">Exclui um [objeto de implantação.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="027d0-124">Deletes a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>|
|[<span data-ttu-id="027d0-125">Listar membros da audiência</span><span class="sxs-lookup"><span data-stu-id="027d0-125">List audience members</span></span>](../api/windowsupdates-deploymentaudience-list-members.md)|<span data-ttu-id="027d0-126">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="027d0-126">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="027d0-127">Listar membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="027d0-127">List members of the deployment audience.</span></span>|
|[<span data-ttu-id="027d0-128">Listar exclusões de audiência</span><span class="sxs-lookup"><span data-stu-id="027d0-128">List audience exclusions</span></span>](../api/windowsupdates-deploymentaudience-list-exclusions.md)|<span data-ttu-id="027d0-129">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="027d0-129">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="027d0-130">Listar exclusões da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="027d0-130">List exclusions from the deployment audience.</span></span>|
|[<span data-ttu-id="027d0-131">Atualizar membros da audiência e exclusões</span><span class="sxs-lookup"><span data-stu-id="027d0-131">Update audience members and exclusions</span></span>](../api/windowsupdates-deploymentaudience-updateaudience.md)|<span data-ttu-id="027d0-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="027d0-132">None</span></span>|<span data-ttu-id="027d0-133">Adicionar ou remover membros e exclusões da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="027d0-133">Add or remove members and exclusions of the deployment audience.</span></span>|

## <a name="properties"></a><span data-ttu-id="027d0-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="027d0-134">Properties</span></span>
|<span data-ttu-id="027d0-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="027d0-135">Property</span></span>|<span data-ttu-id="027d0-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="027d0-136">Type</span></span>|<span data-ttu-id="027d0-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="027d0-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="027d0-138">content</span><span class="sxs-lookup"><span data-stu-id="027d0-138">content</span></span>|[<span data-ttu-id="027d0-139">microsoft.graph.windowsUpdates.deployableContent</span><span class="sxs-lookup"><span data-stu-id="027d0-139">microsoft.graph.windowsUpdates.deployableContent</span></span>](../resources/windowsupdates-deployablecontent.md)|<span data-ttu-id="027d0-140">Especifica qual conteúdo implantar.</span><span class="sxs-lookup"><span data-stu-id="027d0-140">Specifies what content to deploy.</span></span> <span data-ttu-id="027d0-141">Não é possível mudar.</span><span class="sxs-lookup"><span data-stu-id="027d0-141">Cannot be changed.</span></span> <span data-ttu-id="027d0-142">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="027d0-142">Returned by default.</span></span>|
|<span data-ttu-id="027d0-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="027d0-143">createdDateTime</span></span>|<span data-ttu-id="027d0-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="027d0-144">DateTimeOffset</span></span>|<span data-ttu-id="027d0-145">A data e a hora em que a implantação foi criada.</span><span class="sxs-lookup"><span data-stu-id="027d0-145">The date and time the deployment was created.</span></span> <span data-ttu-id="027d0-146">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="027d0-146">Returned by default.</span></span> <span data-ttu-id="027d0-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="027d0-147">Read-only.</span></span>|
|<span data-ttu-id="027d0-148">id</span><span class="sxs-lookup"><span data-stu-id="027d0-148">id</span></span>|<span data-ttu-id="027d0-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="027d0-149">String</span></span>|<span data-ttu-id="027d0-150">O identificador exclusivo da implantação.</span><span class="sxs-lookup"><span data-stu-id="027d0-150">The unique identifier for the deployment.</span></span> <span data-ttu-id="027d0-151">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="027d0-151">Returned by default.</span></span> <span data-ttu-id="027d0-152">Chave.</span><span class="sxs-lookup"><span data-stu-id="027d0-152">Key.</span></span> <span data-ttu-id="027d0-153">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="027d0-153">Not nullable.</span></span> <span data-ttu-id="027d0-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="027d0-154">Read-only.</span></span>|
|<span data-ttu-id="027d0-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="027d0-155">lastModifiedDateTime</span></span>|<span data-ttu-id="027d0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="027d0-156">DateTimeOffset</span></span>|<span data-ttu-id="027d0-157">A data e a hora em que a implantação foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="027d0-157">The date and time the deployment was last modified.</span></span> <span data-ttu-id="027d0-158">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="027d0-158">Returned by default.</span></span> <span data-ttu-id="027d0-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="027d0-159">Read-only.</span></span>|
|<span data-ttu-id="027d0-160">configurações</span><span class="sxs-lookup"><span data-stu-id="027d0-160">settings</span></span>|[<span data-ttu-id="027d0-161">microsoft.graph.windowsUpdates.deploymentSettings</span><span class="sxs-lookup"><span data-stu-id="027d0-161">microsoft.graph.windowsUpdates.deploymentSettings</span></span>](../resources/windowsupdates-deploymentsettings.md)|<span data-ttu-id="027d0-162">Configurações especificado na implantação específica que rege como implantar **conteúdo**.</span><span class="sxs-lookup"><span data-stu-id="027d0-162">Settings specified on the specific deployment governing how to deploy **content**.</span></span> <span data-ttu-id="027d0-163">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="027d0-163">Returned by default.</span></span>|
|<span data-ttu-id="027d0-164">state</span><span class="sxs-lookup"><span data-stu-id="027d0-164">state</span></span>|[<span data-ttu-id="027d0-165">microsoft.graph.windowsUpdates.deploymentState</span><span class="sxs-lookup"><span data-stu-id="027d0-165">microsoft.graph.windowsUpdates.deploymentState</span></span>](../resources/windowsupdates-deploymentstate.md)|<span data-ttu-id="027d0-166">Status de execução da implantação.</span><span class="sxs-lookup"><span data-stu-id="027d0-166">Execution status of the deployment.</span></span> <span data-ttu-id="027d0-167">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="027d0-167">Returned by default.</span></span>|

## <a name="relationships"></a><span data-ttu-id="027d0-168">Relações</span><span class="sxs-lookup"><span data-stu-id="027d0-168">Relationships</span></span>
|<span data-ttu-id="027d0-169">Relação</span><span class="sxs-lookup"><span data-stu-id="027d0-169">Relationship</span></span>|<span data-ttu-id="027d0-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="027d0-170">Type</span></span>|<span data-ttu-id="027d0-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="027d0-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="027d0-172">audience</span><span class="sxs-lookup"><span data-stu-id="027d0-172">audience</span></span>|[<span data-ttu-id="027d0-173">microsoft.graph.windowsUpdates.deploymentAudience</span><span class="sxs-lookup"><span data-stu-id="027d0-173">microsoft.graph.windowsUpdates.deploymentAudience</span></span>](../resources/windowsupdates-deploymentaudience.md)|<span data-ttu-id="027d0-174">Especifica a audiência para a qual o conteúdo é implantado.</span><span class="sxs-lookup"><span data-stu-id="027d0-174">Specifies the audience to which content is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="027d0-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="027d0-175">JSON representation</span></span>
<span data-ttu-id="027d0-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="027d0-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "String (identifier)",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

