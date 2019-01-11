---
title: tipo de recurso de networkManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de rede.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7d91ac60ae52f3317e8148e8bb4adcaf82afac53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806507"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="1cd3a-103">tipo de recurso de networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="1cd3a-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="1cd3a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cd3a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cd3a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cd3a-107">Contém as informações para definir uma condição de gerenciamento de rede.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-107">Contains the information to define a network management condition.</span></span>

<span data-ttu-id="1cd3a-108">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1cd3a-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="1cd3a-109">Methods</span></span>
|<span data-ttu-id="1cd3a-110">Método</span><span class="sxs-lookup"><span data-stu-id="1cd3a-110">Method</span></span>|<span data-ttu-id="1cd3a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1cd3a-111">Return Type</span></span>|<span data-ttu-id="1cd3a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd3a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1cd3a-113">Lista networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="1cd3a-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="1cd3a-114">coleção [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="1cd3a-115">Lista as propriedades e os relacionamentos dos objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="1cd3a-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="1cd3a-116">Obter networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="1cd3a-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="1cd3a-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="1cd3a-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="1cd3a-118">Leia as propriedades e os relacionamentos do objeto [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="1cd3a-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1cd3a-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cd3a-119">Properties</span></span>
|<span data-ttu-id="1cd3a-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cd3a-120">Property</span></span>|<span data-ttu-id="1cd3a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cd3a-121">Type</span></span>|<span data-ttu-id="1cd3a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd3a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd3a-123">id</span><span class="sxs-lookup"><span data-stu-id="1cd3a-123">id</span></span>|<span data-ttu-id="1cd3a-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cd3a-124">String</span></span>|<span data-ttu-id="1cd3a-125">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="1cd3a-126">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-126">System generated value assigned when created.</span></span> <span data-ttu-id="1cd3a-127">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1cd3a-128">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="1cd3a-128">uniqueName</span></span>|<span data-ttu-id="1cd3a-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cd3a-129">String</span></span>|<span data-ttu-id="1cd3a-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-130">Unique name for the management condition.</span></span> <span data-ttu-id="1cd3a-131">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-131">Used in management condition expressions.</span></span> <span data-ttu-id="1cd3a-132">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1cd3a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1cd3a-133">displayName</span></span>|<span data-ttu-id="1cd3a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cd3a-134">String</span></span>|<span data-ttu-id="1cd3a-135">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="1cd3a-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1cd3a-137">description</span><span class="sxs-lookup"><span data-stu-id="1cd3a-137">description</span></span>|<span data-ttu-id="1cd3a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cd3a-138">String</span></span>|<span data-ttu-id="1cd3a-139">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="1cd3a-140">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1cd3a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd3a-141">createdDateTime</span></span>|<span data-ttu-id="1cd3a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd3a-142">DateTimeOffset</span></span>|<span data-ttu-id="1cd3a-143">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-143">The time the management condition was created.</span></span> <span data-ttu-id="1cd3a-144">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-144">Generated service side.</span></span> <span data-ttu-id="1cd3a-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1cd3a-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd3a-146">modifiedDateTime</span></span>|<span data-ttu-id="1cd3a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd3a-147">DateTimeOffset</span></span>|<span data-ttu-id="1cd3a-148">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-148">The time the management condition was last modified.</span></span> <span data-ttu-id="1cd3a-149">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-149">Updated service side.</span></span> <span data-ttu-id="1cd3a-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1cd3a-151">eTag</span><span class="sxs-lookup"><span data-stu-id="1cd3a-151">eTag</span></span>|<span data-ttu-id="1cd3a-152">String</span><span class="sxs-lookup"><span data-stu-id="1cd3a-152">String</span></span>|<span data-ttu-id="1cd3a-153">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-153">ETag of the management condition.</span></span> <span data-ttu-id="1cd3a-154">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-154">Updated service side.</span></span> <span data-ttu-id="1cd3a-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1cd3a-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="1cd3a-156">applicablePlatforms</span></span>|<span data-ttu-id="1cd3a-157">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1cd3a-158">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="1cd3a-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cd3a-160">Relações</span><span class="sxs-lookup"><span data-stu-id="1cd3a-160">Relationships</span></span>
|<span data-ttu-id="1cd3a-161">Relação</span><span class="sxs-lookup"><span data-stu-id="1cd3a-161">Relationship</span></span>|<span data-ttu-id="1cd3a-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cd3a-162">Type</span></span>|<span data-ttu-id="1cd3a-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd3a-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd3a-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="1cd3a-164">managementConditionStatements</span></span>|<span data-ttu-id="1cd3a-165">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="1cd3a-166">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="1cd3a-167">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1cd3a-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cd3a-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cd3a-168">JSON Representation</span></span>
<span data-ttu-id="1cd3a-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cd3a-169">Here is a JSON representation of the resource.</span></span>
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





