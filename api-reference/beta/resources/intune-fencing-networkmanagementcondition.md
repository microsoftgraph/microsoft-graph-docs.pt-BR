---
title: tipo de recurso de networkManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de rede.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4eadaf4e67b7ffe5551fc82376c3a4bb58255f61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415758"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="5c308-103">tipo de recurso de networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="5c308-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="5c308-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5c308-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c308-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5c308-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c308-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5c308-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c308-107">Contém as informações para definir uma condição de gerenciamento de rede.</span><span class="sxs-lookup"><span data-stu-id="5c308-107">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="5c308-108">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5c308-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="5c308-109">Methods</span></span>
|<span data-ttu-id="5c308-110">Método</span><span class="sxs-lookup"><span data-stu-id="5c308-110">Method</span></span>|<span data-ttu-id="5c308-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5c308-111">Return Type</span></span>|<span data-ttu-id="5c308-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c308-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c308-113">Lista networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="5c308-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="5c308-114">coleção [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="5c308-115">Lista as propriedades e os relacionamentos dos objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="5c308-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="5c308-116">Obter networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="5c308-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="5c308-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="5c308-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="5c308-118">Leia as propriedades e os relacionamentos do objeto [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="5c308-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5c308-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c308-119">Properties</span></span>
|<span data-ttu-id="5c308-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c308-120">Property</span></span>|<span data-ttu-id="5c308-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c308-121">Type</span></span>|<span data-ttu-id="5c308-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c308-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c308-123">id</span><span class="sxs-lookup"><span data-stu-id="5c308-123">id</span></span>|<span data-ttu-id="5c308-124">String</span><span class="sxs-lookup"><span data-stu-id="5c308-124">String</span></span>|<span data-ttu-id="5c308-125">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5c308-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="5c308-126">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="5c308-126">System generated value assigned when created.</span></span> <span data-ttu-id="5c308-127">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c308-128">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="5c308-128">uniqueName</span></span>|<span data-ttu-id="5c308-129">String</span><span class="sxs-lookup"><span data-stu-id="5c308-129">String</span></span>|<span data-ttu-id="5c308-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5c308-130">Unique name for the management condition.</span></span> <span data-ttu-id="5c308-131">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5c308-131">Used in management condition expressions.</span></span> <span data-ttu-id="5c308-132">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c308-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5c308-133">displayName</span></span>|<span data-ttu-id="5c308-134">String</span><span class="sxs-lookup"><span data-stu-id="5c308-134">String</span></span>|<span data-ttu-id="5c308-135">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5c308-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="5c308-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c308-137">description</span><span class="sxs-lookup"><span data-stu-id="5c308-137">description</span></span>|<span data-ttu-id="5c308-138">String</span><span class="sxs-lookup"><span data-stu-id="5c308-138">String</span></span>|<span data-ttu-id="5c308-139">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5c308-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="5c308-140">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c308-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c308-141">createdDateTime</span></span>|<span data-ttu-id="5c308-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c308-142">DateTimeOffset</span></span>|<span data-ttu-id="5c308-143">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="5c308-143">The time the management condition was created.</span></span> <span data-ttu-id="5c308-144">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="5c308-144">Generated service side.</span></span> <span data-ttu-id="5c308-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c308-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c308-146">modifiedDateTime</span></span>|<span data-ttu-id="5c308-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c308-147">DateTimeOffset</span></span>|<span data-ttu-id="5c308-148">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5c308-148">The time the management condition was last modified.</span></span> <span data-ttu-id="5c308-149">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="5c308-149">Updated service side.</span></span> <span data-ttu-id="5c308-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c308-151">eTag</span><span class="sxs-lookup"><span data-stu-id="5c308-151">eTag</span></span>|<span data-ttu-id="5c308-152">String</span><span class="sxs-lookup"><span data-stu-id="5c308-152">String</span></span>|<span data-ttu-id="5c308-153">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5c308-153">ETag of the management condition.</span></span> <span data-ttu-id="5c308-154">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="5c308-154">Updated service side.</span></span> <span data-ttu-id="5c308-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="5c308-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="5c308-156">applicablePlatforms</span></span>|<span data-ttu-id="5c308-157">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="5c308-158">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5c308-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="5c308-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c308-160">Relações</span><span class="sxs-lookup"><span data-stu-id="5c308-160">Relationships</span></span>
|<span data-ttu-id="5c308-161">Relação</span><span class="sxs-lookup"><span data-stu-id="5c308-161">Relationship</span></span>|<span data-ttu-id="5c308-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c308-162">Type</span></span>|<span data-ttu-id="5c308-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c308-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c308-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="5c308-164">managementConditionStatements</span></span>|<span data-ttu-id="5c308-165">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="5c308-166">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5c308-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="5c308-167">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5c308-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c308-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c308-168">JSON Representation</span></span>
<span data-ttu-id="5c308-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c308-169">Here is a JSON representation of the resource.</span></span>
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




