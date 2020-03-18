---
title: tipo de recurso managementCondition
description: As condições de gerenciamento são eventos que podem ser acionados dinamicamente, como isolamentos geográficos, cercas de tempo e cercas de rede.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d1adf4538cdfc4bfd819c1e9871c3d3a5a5a800
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783246"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="69abb-103">tipo de recurso managementCondition</span><span class="sxs-lookup"><span data-stu-id="69abb-103">managementCondition resource type</span></span>

> <span data-ttu-id="69abb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69abb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69abb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69abb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69abb-106">As condições de gerenciamento são eventos que podem ser acionados dinamicamente, como isolamentos geográficos, cercas de tempo e cercas de rede.</span><span class="sxs-lookup"><span data-stu-id="69abb-106">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="69abb-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="69abb-107">Methods</span></span>
|<span data-ttu-id="69abb-108">Método</span><span class="sxs-lookup"><span data-stu-id="69abb-108">Method</span></span>|<span data-ttu-id="69abb-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="69abb-109">Return Type</span></span>|<span data-ttu-id="69abb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="69abb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69abb-111">Listar managementConditions</span><span class="sxs-lookup"><span data-stu-id="69abb-111">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="69abb-112">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="69abb-112">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="69abb-113">Listar Propriedades e relações dos objetos [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="69abb-113">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="69abb-114">Obter managementCondition</span><span class="sxs-lookup"><span data-stu-id="69abb-114">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="69abb-115">managementCondition</span><span class="sxs-lookup"><span data-stu-id="69abb-115">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="69abb-116">Leia as propriedades e as relações do objeto [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="69abb-116">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="69abb-117">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="69abb-117">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="69abb-118">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="69abb-118">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="69abb-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="69abb-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="69abb-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69abb-120">Properties</span></span>
|<span data-ttu-id="69abb-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69abb-121">Property</span></span>|<span data-ttu-id="69abb-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="69abb-122">Type</span></span>|<span data-ttu-id="69abb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="69abb-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69abb-124">id</span><span class="sxs-lookup"><span data-stu-id="69abb-124">id</span></span>|<span data-ttu-id="69abb-125">String</span><span class="sxs-lookup"><span data-stu-id="69abb-125">String</span></span>|<span data-ttu-id="69abb-126">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="69abb-126">Unique identifier for the management condition.</span></span> <span data-ttu-id="69abb-127">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="69abb-127">System generated value assigned when created.</span></span>|
|<span data-ttu-id="69abb-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="69abb-128">uniqueName</span></span>|<span data-ttu-id="69abb-129">String</span><span class="sxs-lookup"><span data-stu-id="69abb-129">String</span></span>|<span data-ttu-id="69abb-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="69abb-130">Unique name for the management condition.</span></span> <span data-ttu-id="69abb-131">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="69abb-131">Used in management condition expressions.</span></span>|
|<span data-ttu-id="69abb-132">displayName</span><span class="sxs-lookup"><span data-stu-id="69abb-132">displayName</span></span>|<span data-ttu-id="69abb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abb-133">String</span></span>|<span data-ttu-id="69abb-134">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="69abb-134">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="69abb-135">description</span><span class="sxs-lookup"><span data-stu-id="69abb-135">description</span></span>|<span data-ttu-id="69abb-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69abb-136">String</span></span>|<span data-ttu-id="69abb-137">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="69abb-137">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="69abb-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69abb-138">createdDateTime</span></span>|<span data-ttu-id="69abb-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69abb-139">DateTimeOffset</span></span>|<span data-ttu-id="69abb-140">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="69abb-140">The time the management condition was created.</span></span> <span data-ttu-id="69abb-141">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="69abb-141">Generated service side.</span></span>|
|<span data-ttu-id="69abb-142">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69abb-142">modifiedDateTime</span></span>|<span data-ttu-id="69abb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69abb-143">DateTimeOffset</span></span>|<span data-ttu-id="69abb-144">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="69abb-144">The time the management condition was last modified.</span></span> <span data-ttu-id="69abb-145">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="69abb-145">Updated service side.</span></span>|
|<span data-ttu-id="69abb-146">eTag</span><span class="sxs-lookup"><span data-stu-id="69abb-146">eTag</span></span>|<span data-ttu-id="69abb-147">String</span><span class="sxs-lookup"><span data-stu-id="69abb-147">String</span></span>|<span data-ttu-id="69abb-148">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="69abb-148">ETag of the management condition.</span></span> <span data-ttu-id="69abb-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="69abb-149">Updated service side.</span></span>|
|<span data-ttu-id="69abb-150">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="69abb-150">applicablePlatforms</span></span>|<span data-ttu-id="69abb-151">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="69abb-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="69abb-152">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="69abb-152">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69abb-153">Relações</span><span class="sxs-lookup"><span data-stu-id="69abb-153">Relationships</span></span>
|<span data-ttu-id="69abb-154">Relação</span><span class="sxs-lookup"><span data-stu-id="69abb-154">Relationship</span></span>|<span data-ttu-id="69abb-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="69abb-155">Type</span></span>|<span data-ttu-id="69abb-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="69abb-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69abb-157">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="69abb-157">managementConditionStatements</span></span>|<span data-ttu-id="69abb-158">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="69abb-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="69abb-159">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="69abb-159">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69abb-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69abb-160">JSON Representation</span></span>
<span data-ttu-id="69abb-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69abb-161">Here is a JSON representation of the resource.</span></span>
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



