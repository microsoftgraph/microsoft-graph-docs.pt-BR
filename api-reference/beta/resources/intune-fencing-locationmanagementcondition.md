---
title: tipo de recurso locationManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e03e4c1d31fec4fbcff4f3f610710c1120a6a47
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722877"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="b0994-103">tipo de recurso locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="b0994-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="b0994-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0994-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0994-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0994-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0994-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0994-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0994-107">Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.</span><span class="sxs-lookup"><span data-stu-id="b0994-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="b0994-108">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b0994-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0994-109">Methods</span></span>
|<span data-ttu-id="b0994-110">Método</span><span class="sxs-lookup"><span data-stu-id="b0994-110">Method</span></span>|<span data-ttu-id="b0994-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0994-111">Return Type</span></span>|<span data-ttu-id="b0994-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0994-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0994-113">Listar locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="b0994-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="b0994-114">coleção [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="b0994-115">Listar Propriedades e relações dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="b0994-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="b0994-116">Obter locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="b0994-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="b0994-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="b0994-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="b0994-118">Leia as propriedades e as relações do objeto [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="b0994-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0994-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0994-119">Properties</span></span>
|<span data-ttu-id="b0994-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0994-120">Property</span></span>|<span data-ttu-id="b0994-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0994-121">Type</span></span>|<span data-ttu-id="b0994-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0994-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0994-123">id</span><span class="sxs-lookup"><span data-stu-id="b0994-123">id</span></span>|<span data-ttu-id="b0994-124">String</span><span class="sxs-lookup"><span data-stu-id="b0994-124">String</span></span>|<span data-ttu-id="b0994-125">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b0994-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="b0994-126">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="b0994-126">System generated value assigned when created.</span></span> <span data-ttu-id="b0994-127">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0994-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="b0994-128">uniqueName</span></span>|<span data-ttu-id="b0994-129">String</span><span class="sxs-lookup"><span data-stu-id="b0994-129">String</span></span>|<span data-ttu-id="b0994-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b0994-130">Unique name for the management condition.</span></span> <span data-ttu-id="b0994-131">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b0994-131">Used in management condition expressions.</span></span> <span data-ttu-id="b0994-132">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0994-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b0994-133">displayName</span></span>|<span data-ttu-id="b0994-134">String</span><span class="sxs-lookup"><span data-stu-id="b0994-134">String</span></span>|<span data-ttu-id="b0994-135">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b0994-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="b0994-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0994-137">description</span><span class="sxs-lookup"><span data-stu-id="b0994-137">description</span></span>|<span data-ttu-id="b0994-138">String</span><span class="sxs-lookup"><span data-stu-id="b0994-138">String</span></span>|<span data-ttu-id="b0994-139">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b0994-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="b0994-140">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0994-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0994-141">createdDateTime</span></span>|<span data-ttu-id="b0994-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0994-142">DateTimeOffset</span></span>|<span data-ttu-id="b0994-143">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="b0994-143">The time the management condition was created.</span></span> <span data-ttu-id="b0994-144">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="b0994-144">Generated service side.</span></span> <span data-ttu-id="b0994-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0994-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0994-146">modifiedDateTime</span></span>|<span data-ttu-id="b0994-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0994-147">DateTimeOffset</span></span>|<span data-ttu-id="b0994-148">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b0994-148">The time the management condition was last modified.</span></span> <span data-ttu-id="b0994-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="b0994-149">Updated service side.</span></span> <span data-ttu-id="b0994-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0994-151">eTag</span><span class="sxs-lookup"><span data-stu-id="b0994-151">eTag</span></span>|<span data-ttu-id="b0994-152">String</span><span class="sxs-lookup"><span data-stu-id="b0994-152">String</span></span>|<span data-ttu-id="b0994-153">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b0994-153">ETag of the management condition.</span></span> <span data-ttu-id="b0994-154">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="b0994-154">Updated service side.</span></span> <span data-ttu-id="b0994-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0994-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="b0994-156">applicablePlatforms</span></span>|<span data-ttu-id="b0994-157">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b0994-158">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b0994-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="b0994-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0994-160">Relações</span><span class="sxs-lookup"><span data-stu-id="b0994-160">Relationships</span></span>
|<span data-ttu-id="b0994-161">Relação</span><span class="sxs-lookup"><span data-stu-id="b0994-161">Relationship</span></span>|<span data-ttu-id="b0994-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0994-162">Type</span></span>|<span data-ttu-id="b0994-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0994-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0994-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="b0994-164">managementConditionStatements</span></span>|<span data-ttu-id="b0994-165">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="b0994-166">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b0994-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="b0994-167">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0994-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0994-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0994-168">JSON Representation</span></span>
<span data-ttu-id="b0994-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0994-169">Here is a JSON representation of the resource.</span></span>
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





