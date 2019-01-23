---
title: tipo de recurso de managementCondition
description: Condições de gerenciamento são eventos que podem ser disparados dinamicamente como limites de geo, limites de tempo e limites de rede.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c41b4cb3143349ba0fdd97633a70ec7b38e266ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405853"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="5d8a3-103">tipo de recurso de managementCondition</span><span class="sxs-lookup"><span data-stu-id="5d8a3-103">managementCondition resource type</span></span>

> <span data-ttu-id="5d8a3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d8a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d8a3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d8a3-107">Condições de gerenciamento são eventos que podem ser disparados dinamicamente como limites de geo, limites de tempo e limites de rede.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="5d8a3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5d8a3-108">Methods</span></span>
|<span data-ttu-id="5d8a3-109">Método</span><span class="sxs-lookup"><span data-stu-id="5d8a3-109">Method</span></span>|<span data-ttu-id="5d8a3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5d8a3-110">Return Type</span></span>|<span data-ttu-id="5d8a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d8a3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5d8a3-112">Lista managementConditions</span><span class="sxs-lookup"><span data-stu-id="5d8a3-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="5d8a3-113">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5d8a3-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="5d8a3-114">Lista as propriedades e os relacionamentos dos objetos [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="5d8a3-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="5d8a3-115">Obter managementCondition</span><span class="sxs-lookup"><span data-stu-id="5d8a3-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="5d8a3-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="5d8a3-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="5d8a3-117">Leia as propriedades e os relacionamentos do objeto [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="5d8a3-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="5d8a3-118">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="5d8a3-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="5d8a3-119">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="5d8a3-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="5d8a3-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5d8a3-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5d8a3-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d8a3-121">Properties</span></span>
|<span data-ttu-id="5d8a3-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d8a3-122">Property</span></span>|<span data-ttu-id="5d8a3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d8a3-123">Type</span></span>|<span data-ttu-id="5d8a3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d8a3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d8a3-125">id</span><span class="sxs-lookup"><span data-stu-id="5d8a3-125">id</span></span>|<span data-ttu-id="5d8a3-126">String</span><span class="sxs-lookup"><span data-stu-id="5d8a3-126">String</span></span>|<span data-ttu-id="5d8a3-127">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="5d8a3-128">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="5d8a3-129">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="5d8a3-129">uniqueName</span></span>|<span data-ttu-id="5d8a3-130">String</span><span class="sxs-lookup"><span data-stu-id="5d8a3-130">String</span></span>|<span data-ttu-id="5d8a3-131">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-131">Unique name for the management condition.</span></span> <span data-ttu-id="5d8a3-132">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="5d8a3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5d8a3-133">displayName</span></span>|<span data-ttu-id="5d8a3-134">String</span><span class="sxs-lookup"><span data-stu-id="5d8a3-134">String</span></span>|<span data-ttu-id="5d8a3-135">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="5d8a3-136">description</span><span class="sxs-lookup"><span data-stu-id="5d8a3-136">description</span></span>|<span data-ttu-id="5d8a3-137">String</span><span class="sxs-lookup"><span data-stu-id="5d8a3-137">String</span></span>|<span data-ttu-id="5d8a3-138">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="5d8a3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d8a3-139">createdDateTime</span></span>|<span data-ttu-id="5d8a3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d8a3-140">DateTimeOffset</span></span>|<span data-ttu-id="5d8a3-141">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-141">The time the management condition was created.</span></span> <span data-ttu-id="5d8a3-142">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-142">Generated service side.</span></span>|
|<span data-ttu-id="5d8a3-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d8a3-143">modifiedDateTime</span></span>|<span data-ttu-id="5d8a3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d8a3-144">DateTimeOffset</span></span>|<span data-ttu-id="5d8a3-145">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-145">The time the management condition was last modified.</span></span> <span data-ttu-id="5d8a3-146">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-146">Updated service side.</span></span>|
|<span data-ttu-id="5d8a3-147">eTag</span><span class="sxs-lookup"><span data-stu-id="5d8a3-147">eTag</span></span>|<span data-ttu-id="5d8a3-148">String</span><span class="sxs-lookup"><span data-stu-id="5d8a3-148">String</span></span>|<span data-ttu-id="5d8a3-149">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-149">ETag of the management condition.</span></span> <span data-ttu-id="5d8a3-150">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-150">Updated service side.</span></span>|
|<span data-ttu-id="5d8a3-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="5d8a3-151">applicablePlatforms</span></span>|<span data-ttu-id="5d8a3-152">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="5d8a3-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="5d8a3-153">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d8a3-154">Relações</span><span class="sxs-lookup"><span data-stu-id="5d8a3-154">Relationships</span></span>
|<span data-ttu-id="5d8a3-155">Relação</span><span class="sxs-lookup"><span data-stu-id="5d8a3-155">Relationship</span></span>|<span data-ttu-id="5d8a3-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d8a3-156">Type</span></span>|<span data-ttu-id="5d8a3-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d8a3-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d8a3-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="5d8a3-158">managementConditionStatements</span></span>|<span data-ttu-id="5d8a3-159">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="5d8a3-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="5d8a3-160">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d8a3-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d8a3-161">JSON Representation</span></span>
<span data-ttu-id="5d8a3-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d8a3-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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




