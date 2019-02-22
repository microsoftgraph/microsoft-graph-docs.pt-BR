---
title: tipo de recurso locationManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07bf05fa8ab6f7f7f1ce6e1978645f289ea57a2f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143306"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="1737f-103">tipo de recurso locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="1737f-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="1737f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1737f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1737f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1737f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1737f-106">Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.</span><span class="sxs-lookup"><span data-stu-id="1737f-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="1737f-107">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1737f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1737f-108">Methods</span></span>
|<span data-ttu-id="1737f-109">Método</span><span class="sxs-lookup"><span data-stu-id="1737f-109">Method</span></span>|<span data-ttu-id="1737f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1737f-110">Return Type</span></span>|<span data-ttu-id="1737f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1737f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1737f-112">Listar locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="1737f-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="1737f-113">coleção [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="1737f-114">Listar Propriedades e relações dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="1737f-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="1737f-115">Obter locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="1737f-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="1737f-116">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="1737f-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="1737f-117">Leia as propriedades e as relações do objeto [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="1737f-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1737f-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1737f-118">Properties</span></span>
|<span data-ttu-id="1737f-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1737f-119">Property</span></span>|<span data-ttu-id="1737f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1737f-120">Type</span></span>|<span data-ttu-id="1737f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1737f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1737f-122">id</span><span class="sxs-lookup"><span data-stu-id="1737f-122">id</span></span>|<span data-ttu-id="1737f-123">String</span><span class="sxs-lookup"><span data-stu-id="1737f-123">String</span></span>|<span data-ttu-id="1737f-124">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1737f-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="1737f-125">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="1737f-125">System generated value assigned when created.</span></span> <span data-ttu-id="1737f-126">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1737f-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="1737f-127">uniqueName</span></span>|<span data-ttu-id="1737f-128">String</span><span class="sxs-lookup"><span data-stu-id="1737f-128">String</span></span>|<span data-ttu-id="1737f-129">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1737f-129">Unique name for the management condition.</span></span> <span data-ttu-id="1737f-130">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1737f-130">Used in management condition expressions.</span></span> <span data-ttu-id="1737f-131">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1737f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1737f-132">displayName</span></span>|<span data-ttu-id="1737f-133">String</span><span class="sxs-lookup"><span data-stu-id="1737f-133">String</span></span>|<span data-ttu-id="1737f-134">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1737f-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="1737f-135">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1737f-136">description</span><span class="sxs-lookup"><span data-stu-id="1737f-136">description</span></span>|<span data-ttu-id="1737f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1737f-137">String</span></span>|<span data-ttu-id="1737f-138">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1737f-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="1737f-139">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1737f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1737f-140">createdDateTime</span></span>|<span data-ttu-id="1737f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1737f-141">DateTimeOffset</span></span>|<span data-ttu-id="1737f-142">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="1737f-142">The time the management condition was created.</span></span> <span data-ttu-id="1737f-143">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="1737f-143">Generated service side.</span></span> <span data-ttu-id="1737f-144">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1737f-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1737f-145">modifiedDateTime</span></span>|<span data-ttu-id="1737f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1737f-146">DateTimeOffset</span></span>|<span data-ttu-id="1737f-147">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1737f-147">The time the management condition was last modified.</span></span> <span data-ttu-id="1737f-148">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="1737f-148">Updated service side.</span></span> <span data-ttu-id="1737f-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1737f-150">eTag</span><span class="sxs-lookup"><span data-stu-id="1737f-150">eTag</span></span>|<span data-ttu-id="1737f-151">String</span><span class="sxs-lookup"><span data-stu-id="1737f-151">String</span></span>|<span data-ttu-id="1737f-152">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1737f-152">ETag of the management condition.</span></span> <span data-ttu-id="1737f-153">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="1737f-153">Updated service side.</span></span> <span data-ttu-id="1737f-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1737f-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="1737f-155">applicablePlatforms</span></span>|<span data-ttu-id="1737f-156">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1737f-157">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1737f-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="1737f-158">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1737f-159">Relações</span><span class="sxs-lookup"><span data-stu-id="1737f-159">Relationships</span></span>
|<span data-ttu-id="1737f-160">Relação</span><span class="sxs-lookup"><span data-stu-id="1737f-160">Relationship</span></span>|<span data-ttu-id="1737f-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="1737f-161">Type</span></span>|<span data-ttu-id="1737f-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="1737f-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1737f-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="1737f-163">managementConditionStatements</span></span>|<span data-ttu-id="1737f-164">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="1737f-165">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1737f-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="1737f-166">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1737f-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1737f-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1737f-167">JSON Representation</span></span>
<span data-ttu-id="1737f-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1737f-168">Here is a JSON representation of the resource.</span></span>
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




