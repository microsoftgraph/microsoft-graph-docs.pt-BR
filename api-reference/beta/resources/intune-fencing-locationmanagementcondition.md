---
title: tipo de recurso locationManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f11c23b7e01636fb49273465e340b1085d9b3b2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302702"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="245aa-103">tipo de recurso locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="245aa-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="245aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="245aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="245aa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="245aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="245aa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="245aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="245aa-107">Contém as informações para definir uma condição de gerenciamento de local, uma área de interesse, para monitorar.</span><span class="sxs-lookup"><span data-stu-id="245aa-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="245aa-108">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="245aa-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="245aa-109">Methods</span></span>
|<span data-ttu-id="245aa-110">Método</span><span class="sxs-lookup"><span data-stu-id="245aa-110">Method</span></span>|<span data-ttu-id="245aa-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="245aa-111">Return Type</span></span>|<span data-ttu-id="245aa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="245aa-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="245aa-113">Listar locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="245aa-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="245aa-114">coleção [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="245aa-115">Listar Propriedades e relações dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="245aa-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="245aa-116">Obter locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="245aa-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="245aa-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="245aa-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="245aa-118">Leia as propriedades e as relações do objeto [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="245aa-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="245aa-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="245aa-119">Properties</span></span>
|<span data-ttu-id="245aa-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="245aa-120">Property</span></span>|<span data-ttu-id="245aa-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="245aa-121">Type</span></span>|<span data-ttu-id="245aa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="245aa-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="245aa-123">id</span><span class="sxs-lookup"><span data-stu-id="245aa-123">id</span></span>|<span data-ttu-id="245aa-124">String</span><span class="sxs-lookup"><span data-stu-id="245aa-124">String</span></span>|<span data-ttu-id="245aa-125">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="245aa-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="245aa-126">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="245aa-126">System generated value assigned when created.</span></span> <span data-ttu-id="245aa-127">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="245aa-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="245aa-128">uniqueName</span></span>|<span data-ttu-id="245aa-129">String</span><span class="sxs-lookup"><span data-stu-id="245aa-129">String</span></span>|<span data-ttu-id="245aa-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="245aa-130">Unique name for the management condition.</span></span> <span data-ttu-id="245aa-131">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="245aa-131">Used in management condition expressions.</span></span> <span data-ttu-id="245aa-132">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="245aa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="245aa-133">displayName</span></span>|<span data-ttu-id="245aa-134">String</span><span class="sxs-lookup"><span data-stu-id="245aa-134">String</span></span>|<span data-ttu-id="245aa-135">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="245aa-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="245aa-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="245aa-137">description</span><span class="sxs-lookup"><span data-stu-id="245aa-137">description</span></span>|<span data-ttu-id="245aa-138">String</span><span class="sxs-lookup"><span data-stu-id="245aa-138">String</span></span>|<span data-ttu-id="245aa-139">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="245aa-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="245aa-140">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="245aa-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="245aa-141">createdDateTime</span></span>|<span data-ttu-id="245aa-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="245aa-142">DateTimeOffset</span></span>|<span data-ttu-id="245aa-143">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="245aa-143">The time the management condition was created.</span></span> <span data-ttu-id="245aa-144">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="245aa-144">Generated service side.</span></span> <span data-ttu-id="245aa-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="245aa-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="245aa-146">modifiedDateTime</span></span>|<span data-ttu-id="245aa-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="245aa-147">DateTimeOffset</span></span>|<span data-ttu-id="245aa-148">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="245aa-148">The time the management condition was last modified.</span></span> <span data-ttu-id="245aa-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="245aa-149">Updated service side.</span></span> <span data-ttu-id="245aa-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="245aa-151">eTag</span><span class="sxs-lookup"><span data-stu-id="245aa-151">eTag</span></span>|<span data-ttu-id="245aa-152">String</span><span class="sxs-lookup"><span data-stu-id="245aa-152">String</span></span>|<span data-ttu-id="245aa-153">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="245aa-153">ETag of the management condition.</span></span> <span data-ttu-id="245aa-154">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="245aa-154">Updated service side.</span></span> <span data-ttu-id="245aa-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="245aa-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="245aa-156">applicablePlatforms</span></span>|<span data-ttu-id="245aa-157">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="245aa-158">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="245aa-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="245aa-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="245aa-160">Relações</span><span class="sxs-lookup"><span data-stu-id="245aa-160">Relationships</span></span>
|<span data-ttu-id="245aa-161">Relação</span><span class="sxs-lookup"><span data-stu-id="245aa-161">Relationship</span></span>|<span data-ttu-id="245aa-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="245aa-162">Type</span></span>|<span data-ttu-id="245aa-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="245aa-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="245aa-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="245aa-164">managementConditionStatements</span></span>|<span data-ttu-id="245aa-165">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="245aa-166">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="245aa-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="245aa-167">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="245aa-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="245aa-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="245aa-168">JSON Representation</span></span>
<span data-ttu-id="245aa-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="245aa-169">Here is a JSON representation of the resource.</span></span>
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




