---
title: tipo de recurso locationManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f49359a9c3e527e30944030a8c0969c7c12ce9e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382728"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="7d907-103">tipo de recurso locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="7d907-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="7d907-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d907-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d907-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d907-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d907-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d907-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d907-107">Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.</span><span class="sxs-lookup"><span data-stu-id="7d907-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="7d907-108">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7d907-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d907-109">Methods</span></span>
|<span data-ttu-id="7d907-110">Método</span><span class="sxs-lookup"><span data-stu-id="7d907-110">Method</span></span>|<span data-ttu-id="7d907-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d907-111">Return Type</span></span>|<span data-ttu-id="7d907-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d907-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7d907-113">Listar locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="7d907-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="7d907-114">coleção [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="7d907-115">Listar Propriedades e relações dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="7d907-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="7d907-116">Obter locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="7d907-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="7d907-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="7d907-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="7d907-118">Leia as propriedades e as relações do objeto [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="7d907-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d907-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d907-119">Properties</span></span>
|<span data-ttu-id="7d907-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d907-120">Property</span></span>|<span data-ttu-id="7d907-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d907-121">Type</span></span>|<span data-ttu-id="7d907-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d907-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d907-123">id</span><span class="sxs-lookup"><span data-stu-id="7d907-123">id</span></span>|<span data-ttu-id="7d907-124">String</span><span class="sxs-lookup"><span data-stu-id="7d907-124">String</span></span>|<span data-ttu-id="7d907-125">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7d907-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="7d907-126">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="7d907-126">System generated value assigned when created.</span></span> <span data-ttu-id="7d907-127">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7d907-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="7d907-128">uniqueName</span></span>|<span data-ttu-id="7d907-129">String</span><span class="sxs-lookup"><span data-stu-id="7d907-129">String</span></span>|<span data-ttu-id="7d907-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7d907-130">Unique name for the management condition.</span></span> <span data-ttu-id="7d907-131">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7d907-131">Used in management condition expressions.</span></span> <span data-ttu-id="7d907-132">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7d907-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7d907-133">displayName</span></span>|<span data-ttu-id="7d907-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d907-134">String</span></span>|<span data-ttu-id="7d907-135">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7d907-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="7d907-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7d907-137">description</span><span class="sxs-lookup"><span data-stu-id="7d907-137">description</span></span>|<span data-ttu-id="7d907-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d907-138">String</span></span>|<span data-ttu-id="7d907-139">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7d907-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="7d907-140">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7d907-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d907-141">createdDateTime</span></span>|<span data-ttu-id="7d907-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d907-142">DateTimeOffset</span></span>|<span data-ttu-id="7d907-143">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="7d907-143">The time the management condition was created.</span></span> <span data-ttu-id="7d907-144">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="7d907-144">Generated service side.</span></span> <span data-ttu-id="7d907-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7d907-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d907-146">modifiedDateTime</span></span>|<span data-ttu-id="7d907-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d907-147">DateTimeOffset</span></span>|<span data-ttu-id="7d907-148">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7d907-148">The time the management condition was last modified.</span></span> <span data-ttu-id="7d907-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="7d907-149">Updated service side.</span></span> <span data-ttu-id="7d907-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7d907-151">eTag</span><span class="sxs-lookup"><span data-stu-id="7d907-151">eTag</span></span>|<span data-ttu-id="7d907-152">String</span><span class="sxs-lookup"><span data-stu-id="7d907-152">String</span></span>|<span data-ttu-id="7d907-153">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7d907-153">ETag of the management condition.</span></span> <span data-ttu-id="7d907-154">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="7d907-154">Updated service side.</span></span> <span data-ttu-id="7d907-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="7d907-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="7d907-156">applicablePlatforms</span></span>|<span data-ttu-id="7d907-157">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="7d907-158">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7d907-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="7d907-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d907-160">Relações</span><span class="sxs-lookup"><span data-stu-id="7d907-160">Relationships</span></span>
|<span data-ttu-id="7d907-161">Relação</span><span class="sxs-lookup"><span data-stu-id="7d907-161">Relationship</span></span>|<span data-ttu-id="7d907-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d907-162">Type</span></span>|<span data-ttu-id="7d907-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d907-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d907-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="7d907-164">managementConditionStatements</span></span>|<span data-ttu-id="7d907-165">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="7d907-166">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7d907-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="7d907-167">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="7d907-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d907-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d907-168">JSON Representation</span></span>
<span data-ttu-id="7d907-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d907-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```



