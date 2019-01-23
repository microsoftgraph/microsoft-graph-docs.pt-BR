---
title: tipo de recurso de locationManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de localização, uma área de interesse, para monitorar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c2eddf43696bd9300cc8dcd3408dbcd6fc5a9e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422793"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="d5613-103">tipo de recurso de locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="d5613-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="d5613-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5613-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5613-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5613-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5613-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d5613-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5613-107">Contém as informações para definir uma condição de gerenciamento de localização, uma área de interesse, para monitorar.</span><span class="sxs-lookup"><span data-stu-id="d5613-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="d5613-108">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d5613-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5613-109">Methods</span></span>
|<span data-ttu-id="d5613-110">Método</span><span class="sxs-lookup"><span data-stu-id="d5613-110">Method</span></span>|<span data-ttu-id="d5613-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5613-111">Return Type</span></span>|<span data-ttu-id="d5613-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5613-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5613-113">Lista locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="d5613-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="d5613-114">coleção [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="d5613-115">Lista as propriedades e os relacionamentos dos objetos [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="d5613-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="d5613-116">Obter locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="d5613-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="d5613-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="d5613-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="d5613-118">Leia as propriedades e os relacionamentos do objeto [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="d5613-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5613-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5613-119">Properties</span></span>
|<span data-ttu-id="d5613-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5613-120">Property</span></span>|<span data-ttu-id="d5613-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5613-121">Type</span></span>|<span data-ttu-id="d5613-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5613-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5613-123">id</span><span class="sxs-lookup"><span data-stu-id="d5613-123">id</span></span>|<span data-ttu-id="d5613-124">String</span><span class="sxs-lookup"><span data-stu-id="d5613-124">String</span></span>|<span data-ttu-id="d5613-125">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d5613-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="d5613-126">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="d5613-126">System generated value assigned when created.</span></span> <span data-ttu-id="d5613-127">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5613-128">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="d5613-128">uniqueName</span></span>|<span data-ttu-id="d5613-129">String</span><span class="sxs-lookup"><span data-stu-id="d5613-129">String</span></span>|<span data-ttu-id="d5613-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d5613-130">Unique name for the management condition.</span></span> <span data-ttu-id="d5613-131">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d5613-131">Used in management condition expressions.</span></span> <span data-ttu-id="d5613-132">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5613-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d5613-133">displayName</span></span>|<span data-ttu-id="d5613-134">String</span><span class="sxs-lookup"><span data-stu-id="d5613-134">String</span></span>|<span data-ttu-id="d5613-135">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d5613-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="d5613-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5613-137">description</span><span class="sxs-lookup"><span data-stu-id="d5613-137">description</span></span>|<span data-ttu-id="d5613-138">String</span><span class="sxs-lookup"><span data-stu-id="d5613-138">String</span></span>|<span data-ttu-id="d5613-139">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d5613-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="d5613-140">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5613-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5613-141">createdDateTime</span></span>|<span data-ttu-id="d5613-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5613-142">DateTimeOffset</span></span>|<span data-ttu-id="d5613-143">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="d5613-143">The time the management condition was created.</span></span> <span data-ttu-id="d5613-144">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="d5613-144">Generated service side.</span></span> <span data-ttu-id="d5613-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5613-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5613-146">modifiedDateTime</span></span>|<span data-ttu-id="d5613-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5613-147">DateTimeOffset</span></span>|<span data-ttu-id="d5613-148">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d5613-148">The time the management condition was last modified.</span></span> <span data-ttu-id="d5613-149">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="d5613-149">Updated service side.</span></span> <span data-ttu-id="d5613-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5613-151">eTag</span><span class="sxs-lookup"><span data-stu-id="d5613-151">eTag</span></span>|<span data-ttu-id="d5613-152">String</span><span class="sxs-lookup"><span data-stu-id="d5613-152">String</span></span>|<span data-ttu-id="d5613-153">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d5613-153">ETag of the management condition.</span></span> <span data-ttu-id="d5613-154">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="d5613-154">Updated service side.</span></span> <span data-ttu-id="d5613-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="d5613-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="d5613-156">applicablePlatforms</span></span>|<span data-ttu-id="d5613-157">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="d5613-158">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d5613-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="d5613-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5613-160">Relações</span><span class="sxs-lookup"><span data-stu-id="d5613-160">Relationships</span></span>
|<span data-ttu-id="d5613-161">Relação</span><span class="sxs-lookup"><span data-stu-id="d5613-161">Relationship</span></span>|<span data-ttu-id="d5613-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5613-162">Type</span></span>|<span data-ttu-id="d5613-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5613-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5613-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="d5613-164">managementConditionStatements</span></span>|<span data-ttu-id="d5613-165">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="d5613-166">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d5613-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="d5613-167">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="d5613-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5613-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5613-168">JSON Representation</span></span>
<span data-ttu-id="d5613-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5613-169">Here is a JSON representation of the resource.</span></span>
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




