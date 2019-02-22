---
title: tipo de recurso managementCondition
description: As condições de gerenciamento são eventos que podem ser acionados dinamicamente, como isolamentos geográficos, cercas de tempo e cercas de rede.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 594716867cec1dcef9e0fee87af21fb63af99df0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163102"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="c604a-103">tipo de recurso managementCondition</span><span class="sxs-lookup"><span data-stu-id="c604a-103">managementCondition resource type</span></span>

> <span data-ttu-id="c604a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c604a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c604a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c604a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c604a-106">As condições de gerenciamento são eventos que podem ser acionados dinamicamente, como isolamentos geográficos, cercas de tempo e cercas de rede.</span><span class="sxs-lookup"><span data-stu-id="c604a-106">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="c604a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c604a-107">Methods</span></span>
|<span data-ttu-id="c604a-108">Método</span><span class="sxs-lookup"><span data-stu-id="c604a-108">Method</span></span>|<span data-ttu-id="c604a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c604a-109">Return Type</span></span>|<span data-ttu-id="c604a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c604a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c604a-111">Listar managementConditions</span><span class="sxs-lookup"><span data-stu-id="c604a-111">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="c604a-112">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="c604a-112">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="c604a-113">Listar Propriedades e relações dos objetos [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="c604a-113">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="c604a-114">Obter managementCondition</span><span class="sxs-lookup"><span data-stu-id="c604a-114">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="c604a-115">managementCondition</span><span class="sxs-lookup"><span data-stu-id="c604a-115">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="c604a-116">Leia as propriedades e as relações do objeto [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="c604a-116">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="c604a-117">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="c604a-117">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="c604a-118">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="c604a-118">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="c604a-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c604a-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c604a-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c604a-120">Properties</span></span>
|<span data-ttu-id="c604a-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c604a-121">Property</span></span>|<span data-ttu-id="c604a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c604a-122">Type</span></span>|<span data-ttu-id="c604a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c604a-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c604a-124">id</span><span class="sxs-lookup"><span data-stu-id="c604a-124">id</span></span>|<span data-ttu-id="c604a-125">String</span><span class="sxs-lookup"><span data-stu-id="c604a-125">String</span></span>|<span data-ttu-id="c604a-126">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c604a-126">Unique identifier for the management condition.</span></span> <span data-ttu-id="c604a-127">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="c604a-127">System generated value assigned when created.</span></span>|
|<span data-ttu-id="c604a-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="c604a-128">uniqueName</span></span>|<span data-ttu-id="c604a-129">String</span><span class="sxs-lookup"><span data-stu-id="c604a-129">String</span></span>|<span data-ttu-id="c604a-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c604a-130">Unique name for the management condition.</span></span> <span data-ttu-id="c604a-131">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c604a-131">Used in management condition expressions.</span></span>|
|<span data-ttu-id="c604a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c604a-132">displayName</span></span>|<span data-ttu-id="c604a-133">String</span><span class="sxs-lookup"><span data-stu-id="c604a-133">String</span></span>|<span data-ttu-id="c604a-134">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c604a-134">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="c604a-135">description</span><span class="sxs-lookup"><span data-stu-id="c604a-135">description</span></span>|<span data-ttu-id="c604a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c604a-136">String</span></span>|<span data-ttu-id="c604a-137">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c604a-137">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="c604a-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c604a-138">createdDateTime</span></span>|<span data-ttu-id="c604a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c604a-139">DateTimeOffset</span></span>|<span data-ttu-id="c604a-140">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="c604a-140">The time the management condition was created.</span></span> <span data-ttu-id="c604a-141">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="c604a-141">Generated service side.</span></span>|
|<span data-ttu-id="c604a-142">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c604a-142">modifiedDateTime</span></span>|<span data-ttu-id="c604a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c604a-143">DateTimeOffset</span></span>|<span data-ttu-id="c604a-144">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c604a-144">The time the management condition was last modified.</span></span> <span data-ttu-id="c604a-145">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="c604a-145">Updated service side.</span></span>|
|<span data-ttu-id="c604a-146">eTag</span><span class="sxs-lookup"><span data-stu-id="c604a-146">eTag</span></span>|<span data-ttu-id="c604a-147">String</span><span class="sxs-lookup"><span data-stu-id="c604a-147">String</span></span>|<span data-ttu-id="c604a-148">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c604a-148">ETag of the management condition.</span></span> <span data-ttu-id="c604a-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="c604a-149">Updated service side.</span></span>|
|<span data-ttu-id="c604a-150">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="c604a-150">applicablePlatforms</span></span>|<span data-ttu-id="c604a-151">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="c604a-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="c604a-152">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c604a-152">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c604a-153">Relações</span><span class="sxs-lookup"><span data-stu-id="c604a-153">Relationships</span></span>
|<span data-ttu-id="c604a-154">Relação</span><span class="sxs-lookup"><span data-stu-id="c604a-154">Relationship</span></span>|<span data-ttu-id="c604a-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="c604a-155">Type</span></span>|<span data-ttu-id="c604a-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="c604a-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c604a-157">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="c604a-157">managementConditionStatements</span></span>|<span data-ttu-id="c604a-158">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="c604a-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="c604a-159">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c604a-159">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c604a-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c604a-160">JSON Representation</span></span>
<span data-ttu-id="c604a-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c604a-161">Here is a JSON representation of the resource.</span></span>
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




