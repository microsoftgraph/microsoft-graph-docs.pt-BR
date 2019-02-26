---
title: tipo de recurso networkManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de rede.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 909eaa89a8303948cd97ba47299146b575e32c9f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164831"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="fee41-103">tipo de recurso networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="fee41-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="fee41-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fee41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fee41-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fee41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fee41-106">Contém as informações para definir uma condição de gerenciamento de rede.</span><span class="sxs-lookup"><span data-stu-id="fee41-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="fee41-107">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="fee41-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="fee41-108">Methods</span></span>
|<span data-ttu-id="fee41-109">Método</span><span class="sxs-lookup"><span data-stu-id="fee41-109">Method</span></span>|<span data-ttu-id="fee41-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fee41-110">Return Type</span></span>|<span data-ttu-id="fee41-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fee41-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fee41-112">Listar networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="fee41-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="fee41-113">coleção [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="fee41-114">Listar Propriedades e relações dos objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="fee41-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="fee41-115">Obter networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="fee41-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="fee41-116">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="fee41-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="fee41-117">Leia as propriedades e as relações do objeto [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="fee41-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fee41-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fee41-118">Properties</span></span>
|<span data-ttu-id="fee41-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fee41-119">Property</span></span>|<span data-ttu-id="fee41-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="fee41-120">Type</span></span>|<span data-ttu-id="fee41-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fee41-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fee41-122">id</span><span class="sxs-lookup"><span data-stu-id="fee41-122">id</span></span>|<span data-ttu-id="fee41-123">String</span><span class="sxs-lookup"><span data-stu-id="fee41-123">String</span></span>|<span data-ttu-id="fee41-124">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="fee41-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="fee41-125">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="fee41-125">System generated value assigned when created.</span></span> <span data-ttu-id="fee41-126">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fee41-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="fee41-127">uniqueName</span></span>|<span data-ttu-id="fee41-128">String</span><span class="sxs-lookup"><span data-stu-id="fee41-128">String</span></span>|<span data-ttu-id="fee41-129">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="fee41-129">Unique name for the management condition.</span></span> <span data-ttu-id="fee41-130">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="fee41-130">Used in management condition expressions.</span></span> <span data-ttu-id="fee41-131">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fee41-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fee41-132">displayName</span></span>|<span data-ttu-id="fee41-133">String</span><span class="sxs-lookup"><span data-stu-id="fee41-133">String</span></span>|<span data-ttu-id="fee41-134">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="fee41-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="fee41-135">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fee41-136">description</span><span class="sxs-lookup"><span data-stu-id="fee41-136">description</span></span>|<span data-ttu-id="fee41-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fee41-137">String</span></span>|<span data-ttu-id="fee41-138">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="fee41-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="fee41-139">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fee41-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fee41-140">createdDateTime</span></span>|<span data-ttu-id="fee41-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fee41-141">DateTimeOffset</span></span>|<span data-ttu-id="fee41-142">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="fee41-142">The time the management condition was created.</span></span> <span data-ttu-id="fee41-143">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="fee41-143">Generated service side.</span></span> <span data-ttu-id="fee41-144">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fee41-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fee41-145">modifiedDateTime</span></span>|<span data-ttu-id="fee41-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fee41-146">DateTimeOffset</span></span>|<span data-ttu-id="fee41-147">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fee41-147">The time the management condition was last modified.</span></span> <span data-ttu-id="fee41-148">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="fee41-148">Updated service side.</span></span> <span data-ttu-id="fee41-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fee41-150">eTag</span><span class="sxs-lookup"><span data-stu-id="fee41-150">eTag</span></span>|<span data-ttu-id="fee41-151">String</span><span class="sxs-lookup"><span data-stu-id="fee41-151">String</span></span>|<span data-ttu-id="fee41-152">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="fee41-152">ETag of the management condition.</span></span> <span data-ttu-id="fee41-153">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="fee41-153">Updated service side.</span></span> <span data-ttu-id="fee41-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fee41-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="fee41-155">applicablePlatforms</span></span>|<span data-ttu-id="fee41-156">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="fee41-157">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="fee41-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="fee41-158">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="fee41-159">Relações</span><span class="sxs-lookup"><span data-stu-id="fee41-159">Relationships</span></span>
|<span data-ttu-id="fee41-160">Relação</span><span class="sxs-lookup"><span data-stu-id="fee41-160">Relationship</span></span>|<span data-ttu-id="fee41-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="fee41-161">Type</span></span>|<span data-ttu-id="fee41-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="fee41-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fee41-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="fee41-163">managementConditionStatements</span></span>|<span data-ttu-id="fee41-164">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="fee41-165">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="fee41-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="fee41-166">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fee41-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fee41-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fee41-167">JSON Representation</span></span>
<span data-ttu-id="fee41-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fee41-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
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




