---
title: tipo de recurso locationManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e633e0dab4069997843e733431a601697b23dd30
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011117"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="34f7a-103">tipo de recurso locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="34f7a-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="34f7a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34f7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34f7a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34f7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34f7a-106">Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.</span><span class="sxs-lookup"><span data-stu-id="34f7a-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="34f7a-107">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="34f7a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="34f7a-108">Methods</span></span>
|<span data-ttu-id="34f7a-109">Método</span><span class="sxs-lookup"><span data-stu-id="34f7a-109">Method</span></span>|<span data-ttu-id="34f7a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="34f7a-110">Return Type</span></span>|<span data-ttu-id="34f7a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="34f7a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34f7a-112">Listar locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="34f7a-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="34f7a-113">coleção [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="34f7a-114">Listar Propriedades e relações dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="34f7a-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="34f7a-115">Obter locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="34f7a-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="34f7a-116">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="34f7a-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="34f7a-117">Leia as propriedades e as relações do objeto [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="34f7a-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="34f7a-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34f7a-118">Properties</span></span>
|<span data-ttu-id="34f7a-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34f7a-119">Property</span></span>|<span data-ttu-id="34f7a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="34f7a-120">Type</span></span>|<span data-ttu-id="34f7a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="34f7a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34f7a-122">id</span><span class="sxs-lookup"><span data-stu-id="34f7a-122">id</span></span>|<span data-ttu-id="34f7a-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34f7a-123">String</span></span>|<span data-ttu-id="34f7a-124">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="34f7a-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="34f7a-125">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="34f7a-125">System generated value assigned when created.</span></span> <span data-ttu-id="34f7a-126">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="34f7a-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="34f7a-127">uniqueName</span></span>|<span data-ttu-id="34f7a-128">String</span><span class="sxs-lookup"><span data-stu-id="34f7a-128">String</span></span>|<span data-ttu-id="34f7a-129">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="34f7a-129">Unique name for the management condition.</span></span> <span data-ttu-id="34f7a-130">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="34f7a-130">Used in management condition expressions.</span></span> <span data-ttu-id="34f7a-131">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="34f7a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="34f7a-132">displayName</span></span>|<span data-ttu-id="34f7a-133">String</span><span class="sxs-lookup"><span data-stu-id="34f7a-133">String</span></span>|<span data-ttu-id="34f7a-134">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="34f7a-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="34f7a-135">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="34f7a-136">descrição</span><span class="sxs-lookup"><span data-stu-id="34f7a-136">description</span></span>|<span data-ttu-id="34f7a-137">String</span><span class="sxs-lookup"><span data-stu-id="34f7a-137">String</span></span>|<span data-ttu-id="34f7a-138">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="34f7a-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="34f7a-139">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="34f7a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34f7a-140">createdDateTime</span></span>|<span data-ttu-id="34f7a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34f7a-141">DateTimeOffset</span></span>|<span data-ttu-id="34f7a-142">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="34f7a-142">The time the management condition was created.</span></span> <span data-ttu-id="34f7a-143">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="34f7a-143">Generated service side.</span></span> <span data-ttu-id="34f7a-144">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="34f7a-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34f7a-145">modifiedDateTime</span></span>|<span data-ttu-id="34f7a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34f7a-146">DateTimeOffset</span></span>|<span data-ttu-id="34f7a-147">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="34f7a-147">The time the management condition was last modified.</span></span> <span data-ttu-id="34f7a-148">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="34f7a-148">Updated service side.</span></span> <span data-ttu-id="34f7a-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="34f7a-150">eTag</span><span class="sxs-lookup"><span data-stu-id="34f7a-150">eTag</span></span>|<span data-ttu-id="34f7a-151">String</span><span class="sxs-lookup"><span data-stu-id="34f7a-151">String</span></span>|<span data-ttu-id="34f7a-152">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="34f7a-152">ETag of the management condition.</span></span> <span data-ttu-id="34f7a-153">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="34f7a-153">Updated service side.</span></span> <span data-ttu-id="34f7a-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="34f7a-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="34f7a-155">applicablePlatforms</span></span>|<span data-ttu-id="34f7a-156">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="34f7a-157">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="34f7a-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="34f7a-158">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="34f7a-159">Relações</span><span class="sxs-lookup"><span data-stu-id="34f7a-159">Relationships</span></span>
|<span data-ttu-id="34f7a-160">Relação</span><span class="sxs-lookup"><span data-stu-id="34f7a-160">Relationship</span></span>|<span data-ttu-id="34f7a-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="34f7a-161">Type</span></span>|<span data-ttu-id="34f7a-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="34f7a-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34f7a-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="34f7a-163">managementConditionStatements</span></span>|<span data-ttu-id="34f7a-164">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="34f7a-165">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="34f7a-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="34f7a-166">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="34f7a-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34f7a-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34f7a-167">JSON Representation</span></span>
<span data-ttu-id="34f7a-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34f7a-168">Here is a JSON representation of the resource.</span></span>
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





