---
title: tipo de recurso networkManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de rede.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f824669ff4b5adc8b2ae8c4924f4389514d7e78
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728092"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="2d47d-103">tipo de recurso networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="2d47d-103">networkManagementCondition resource type</span></span>

<span data-ttu-id="2d47d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d47d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d47d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d47d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d47d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d47d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d47d-107">Contém as informações para definir uma condição de gerenciamento de rede.</span><span class="sxs-lookup"><span data-stu-id="2d47d-107">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="2d47d-108">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2d47d-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="2d47d-109">Methods</span></span>
|<span data-ttu-id="2d47d-110">Método</span><span class="sxs-lookup"><span data-stu-id="2d47d-110">Method</span></span>|<span data-ttu-id="2d47d-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2d47d-111">Return Type</span></span>|<span data-ttu-id="2d47d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d47d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2d47d-113">Listar networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="2d47d-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="2d47d-114">coleção [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="2d47d-115">Listar Propriedades e relações dos objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="2d47d-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="2d47d-116">Obter networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="2d47d-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="2d47d-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="2d47d-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="2d47d-118">Leia as propriedades e as relações do objeto [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="2d47d-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d47d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d47d-119">Properties</span></span>
|<span data-ttu-id="2d47d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d47d-120">Property</span></span>|<span data-ttu-id="2d47d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d47d-121">Type</span></span>|<span data-ttu-id="2d47d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d47d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d47d-123">id</span><span class="sxs-lookup"><span data-stu-id="2d47d-123">id</span></span>|<span data-ttu-id="2d47d-124">String</span><span class="sxs-lookup"><span data-stu-id="2d47d-124">String</span></span>|<span data-ttu-id="2d47d-125">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2d47d-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="2d47d-126">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="2d47d-126">System generated value assigned when created.</span></span> <span data-ttu-id="2d47d-127">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2d47d-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="2d47d-128">uniqueName</span></span>|<span data-ttu-id="2d47d-129">String</span><span class="sxs-lookup"><span data-stu-id="2d47d-129">String</span></span>|<span data-ttu-id="2d47d-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2d47d-130">Unique name for the management condition.</span></span> <span data-ttu-id="2d47d-131">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2d47d-131">Used in management condition expressions.</span></span> <span data-ttu-id="2d47d-132">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2d47d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2d47d-133">displayName</span></span>|<span data-ttu-id="2d47d-134">String</span><span class="sxs-lookup"><span data-stu-id="2d47d-134">String</span></span>|<span data-ttu-id="2d47d-135">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2d47d-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="2d47d-136">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2d47d-137">description</span><span class="sxs-lookup"><span data-stu-id="2d47d-137">description</span></span>|<span data-ttu-id="2d47d-138">String</span><span class="sxs-lookup"><span data-stu-id="2d47d-138">String</span></span>|<span data-ttu-id="2d47d-139">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2d47d-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="2d47d-140">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2d47d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d47d-141">createdDateTime</span></span>|<span data-ttu-id="2d47d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d47d-142">DateTimeOffset</span></span>|<span data-ttu-id="2d47d-143">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="2d47d-143">The time the management condition was created.</span></span> <span data-ttu-id="2d47d-144">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="2d47d-144">Generated service side.</span></span> <span data-ttu-id="2d47d-145">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2d47d-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d47d-146">modifiedDateTime</span></span>|<span data-ttu-id="2d47d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d47d-147">DateTimeOffset</span></span>|<span data-ttu-id="2d47d-148">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2d47d-148">The time the management condition was last modified.</span></span> <span data-ttu-id="2d47d-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="2d47d-149">Updated service side.</span></span> <span data-ttu-id="2d47d-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2d47d-151">eTag</span><span class="sxs-lookup"><span data-stu-id="2d47d-151">eTag</span></span>|<span data-ttu-id="2d47d-152">String</span><span class="sxs-lookup"><span data-stu-id="2d47d-152">String</span></span>|<span data-ttu-id="2d47d-153">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2d47d-153">ETag of the management condition.</span></span> <span data-ttu-id="2d47d-154">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="2d47d-154">Updated service side.</span></span> <span data-ttu-id="2d47d-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2d47d-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="2d47d-156">applicablePlatforms</span></span>|<span data-ttu-id="2d47d-157">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="2d47d-158">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2d47d-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="2d47d-159">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d47d-160">Relações</span><span class="sxs-lookup"><span data-stu-id="2d47d-160">Relationships</span></span>
|<span data-ttu-id="2d47d-161">Relação</span><span class="sxs-lookup"><span data-stu-id="2d47d-161">Relationship</span></span>|<span data-ttu-id="2d47d-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d47d-162">Type</span></span>|<span data-ttu-id="2d47d-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d47d-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d47d-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="2d47d-164">managementConditionStatements</span></span>|<span data-ttu-id="2d47d-165">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="2d47d-166">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2d47d-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="2d47d-167">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2d47d-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d47d-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d47d-168">JSON Representation</span></span>
<span data-ttu-id="2d47d-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d47d-169">Here is a JSON representation of the resource.</span></span>
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





