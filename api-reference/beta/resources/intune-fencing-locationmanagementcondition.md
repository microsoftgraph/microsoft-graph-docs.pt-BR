---
title: tipo de recurso de locationManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de localização, uma área de interesse, para monitorar.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 541cf74decad641f6dc7751945e1d0ffceee1366
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922974"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="e209b-103">tipo de recurso de locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="e209b-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="e209b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e209b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e209b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e209b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e209b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e209b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e209b-107">Contém as informações para definir uma condição de gerenciamento de localização, uma área de interesse, para monitorar.</span><span class="sxs-lookup"><span data-stu-id="e209b-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>

<span data-ttu-id="e209b-108">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e209b-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="e209b-109">Methods</span></span>
|<span data-ttu-id="e209b-110">Método</span><span class="sxs-lookup"><span data-stu-id="e209b-110">Method</span></span>|<span data-ttu-id="e209b-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e209b-111">Return Type</span></span>|<span data-ttu-id="e209b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e209b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e209b-113">Lista locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="e209b-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="e209b-114">coleção [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="e209b-115">Lista as propriedades e os relacionamentos dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="e209b-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="e209b-116">Obter locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="e209b-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="e209b-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="e209b-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="e209b-118">Leia as propriedades e os relacionamentos do objeto [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="e209b-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e209b-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e209b-119">Properties</span></span>
|<span data-ttu-id="e209b-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e209b-120">Property</span></span>|<span data-ttu-id="e209b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e209b-121">Type</span></span>|<span data-ttu-id="e209b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e209b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e209b-123">id</span><span class="sxs-lookup"><span data-stu-id="e209b-123">id</span></span>|<span data-ttu-id="e209b-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e209b-124">String</span></span>|<span data-ttu-id="e209b-125">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e209b-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="e209b-126">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="e209b-126">System generated value assigned when created.</span></span> <span data-ttu-id="e209b-127">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e209b-128">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="e209b-128">uniqueName</span></span>|<span data-ttu-id="e209b-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e209b-129">String</span></span>|<span data-ttu-id="e209b-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e209b-130">Unique name for the management condition.</span></span> <span data-ttu-id="e209b-131">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e209b-131">Used in management condition expressions.</span></span> <span data-ttu-id="e209b-132">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e209b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e209b-133">displayName</span></span>|<span data-ttu-id="e209b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e209b-134">String</span></span>|<span data-ttu-id="e209b-135">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e209b-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="e209b-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e209b-137">description</span><span class="sxs-lookup"><span data-stu-id="e209b-137">description</span></span>|<span data-ttu-id="e209b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e209b-138">String</span></span>|<span data-ttu-id="e209b-139">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e209b-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="e209b-140">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e209b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e209b-141">createdDateTime</span></span>|<span data-ttu-id="e209b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e209b-142">DateTimeOffset</span></span>|<span data-ttu-id="e209b-143">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="e209b-143">The time the management condition was created.</span></span> <span data-ttu-id="e209b-144">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="e209b-144">Generated service side.</span></span> <span data-ttu-id="e209b-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e209b-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e209b-146">modifiedDateTime</span></span>|<span data-ttu-id="e209b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e209b-147">DateTimeOffset</span></span>|<span data-ttu-id="e209b-148">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e209b-148">The time the management condition was last modified.</span></span> <span data-ttu-id="e209b-149">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="e209b-149">Updated service side.</span></span> <span data-ttu-id="e209b-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e209b-151">eTag</span><span class="sxs-lookup"><span data-stu-id="e209b-151">eTag</span></span>|<span data-ttu-id="e209b-152">String</span><span class="sxs-lookup"><span data-stu-id="e209b-152">String</span></span>|<span data-ttu-id="e209b-153">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e209b-153">ETag of the management condition.</span></span> <span data-ttu-id="e209b-154">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="e209b-154">Updated service side.</span></span> <span data-ttu-id="e209b-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="e209b-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="e209b-156">applicablePlatforms</span></span>|<span data-ttu-id="e209b-157">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="e209b-158">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e209b-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="e209b-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e209b-160">Relações</span><span class="sxs-lookup"><span data-stu-id="e209b-160">Relationships</span></span>
|<span data-ttu-id="e209b-161">Relação</span><span class="sxs-lookup"><span data-stu-id="e209b-161">Relationship</span></span>|<span data-ttu-id="e209b-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="e209b-162">Type</span></span>|<span data-ttu-id="e209b-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="e209b-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e209b-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="e209b-164">managementConditionStatements</span></span>|<span data-ttu-id="e209b-165">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="e209b-166">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e209b-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="e209b-167">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="e209b-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e209b-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e209b-168">JSON Representation</span></span>
<span data-ttu-id="e209b-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e209b-169">Here is a JSON representation of the resource.</span></span>
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





