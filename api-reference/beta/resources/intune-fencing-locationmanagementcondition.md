---
title: tipo de recurso locationManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 56e9c10d8d9d53a9e0009b6a70210da6d7873065
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783253"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="20386-103">tipo de recurso locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="20386-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="20386-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20386-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20386-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20386-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20386-106">Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.</span><span class="sxs-lookup"><span data-stu-id="20386-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="20386-107">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="20386-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="20386-108">Methods</span></span>
|<span data-ttu-id="20386-109">Método</span><span class="sxs-lookup"><span data-stu-id="20386-109">Method</span></span>|<span data-ttu-id="20386-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="20386-110">Return Type</span></span>|<span data-ttu-id="20386-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="20386-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="20386-112">Listar locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="20386-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="20386-113">coleção [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="20386-114">Listar Propriedades e relações dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="20386-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="20386-115">Obter locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="20386-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="20386-116">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="20386-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="20386-117">Leia as propriedades e as relações do objeto [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="20386-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="20386-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20386-118">Properties</span></span>
|<span data-ttu-id="20386-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20386-119">Property</span></span>|<span data-ttu-id="20386-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="20386-120">Type</span></span>|<span data-ttu-id="20386-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="20386-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20386-122">id</span><span class="sxs-lookup"><span data-stu-id="20386-122">id</span></span>|<span data-ttu-id="20386-123">String</span><span class="sxs-lookup"><span data-stu-id="20386-123">String</span></span>|<span data-ttu-id="20386-124">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="20386-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="20386-125">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="20386-125">System generated value assigned when created.</span></span> <span data-ttu-id="20386-126">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="20386-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="20386-127">uniqueName</span></span>|<span data-ttu-id="20386-128">String</span><span class="sxs-lookup"><span data-stu-id="20386-128">String</span></span>|<span data-ttu-id="20386-129">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="20386-129">Unique name for the management condition.</span></span> <span data-ttu-id="20386-130">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="20386-130">Used in management condition expressions.</span></span> <span data-ttu-id="20386-131">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="20386-132">displayName</span><span class="sxs-lookup"><span data-stu-id="20386-132">displayName</span></span>|<span data-ttu-id="20386-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20386-133">String</span></span>|<span data-ttu-id="20386-134">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="20386-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="20386-135">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="20386-136">description</span><span class="sxs-lookup"><span data-stu-id="20386-136">description</span></span>|<span data-ttu-id="20386-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20386-137">String</span></span>|<span data-ttu-id="20386-138">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="20386-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="20386-139">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="20386-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20386-140">createdDateTime</span></span>|<span data-ttu-id="20386-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20386-141">DateTimeOffset</span></span>|<span data-ttu-id="20386-142">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="20386-142">The time the management condition was created.</span></span> <span data-ttu-id="20386-143">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="20386-143">Generated service side.</span></span> <span data-ttu-id="20386-144">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="20386-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20386-145">modifiedDateTime</span></span>|<span data-ttu-id="20386-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20386-146">DateTimeOffset</span></span>|<span data-ttu-id="20386-147">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="20386-147">The time the management condition was last modified.</span></span> <span data-ttu-id="20386-148">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="20386-148">Updated service side.</span></span> <span data-ttu-id="20386-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="20386-150">eTag</span><span class="sxs-lookup"><span data-stu-id="20386-150">eTag</span></span>|<span data-ttu-id="20386-151">String</span><span class="sxs-lookup"><span data-stu-id="20386-151">String</span></span>|<span data-ttu-id="20386-152">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="20386-152">ETag of the management condition.</span></span> <span data-ttu-id="20386-153">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="20386-153">Updated service side.</span></span> <span data-ttu-id="20386-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="20386-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="20386-155">applicablePlatforms</span></span>|<span data-ttu-id="20386-156">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="20386-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="20386-157">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="20386-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="20386-158">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="20386-159">Relações</span><span class="sxs-lookup"><span data-stu-id="20386-159">Relationships</span></span>
|<span data-ttu-id="20386-160">Relação</span><span class="sxs-lookup"><span data-stu-id="20386-160">Relationship</span></span>|<span data-ttu-id="20386-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="20386-161">Type</span></span>|<span data-ttu-id="20386-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="20386-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20386-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="20386-163">managementConditionStatements</span></span>|<span data-ttu-id="20386-164">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="20386-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="20386-165">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="20386-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="20386-166">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="20386-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20386-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20386-167">JSON Representation</span></span>
<span data-ttu-id="20386-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20386-168">Here is a JSON representation of the resource.</span></span>
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



