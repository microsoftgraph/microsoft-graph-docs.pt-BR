---
title: tipo de recurso managementCondition
description: As condições de gerenciamento são eventos que podem ser acionados dinamicamente, como isolamentos geográficos, cercas de tempo e cercas de rede.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 582af8906fe9948b87a5526ca53a1c2592a0d083
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331683"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="39bdc-103">tipo de recurso managementCondition</span><span class="sxs-lookup"><span data-stu-id="39bdc-103">managementCondition resource type</span></span>

> <span data-ttu-id="39bdc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39bdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39bdc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39bdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39bdc-106">As condições de gerenciamento são eventos que podem ser acionados dinamicamente, como isolamentos geográficos, cercas de tempo e cercas de rede.</span><span class="sxs-lookup"><span data-stu-id="39bdc-106">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="39bdc-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="39bdc-107">Methods</span></span>
|<span data-ttu-id="39bdc-108">Método</span><span class="sxs-lookup"><span data-stu-id="39bdc-108">Method</span></span>|<span data-ttu-id="39bdc-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="39bdc-109">Return Type</span></span>|<span data-ttu-id="39bdc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="39bdc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39bdc-111">Listar managementConditions</span><span class="sxs-lookup"><span data-stu-id="39bdc-111">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="39bdc-112">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="39bdc-112">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="39bdc-113">Listar Propriedades e relações dos objetos [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="39bdc-113">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="39bdc-114">Obter managementCondition</span><span class="sxs-lookup"><span data-stu-id="39bdc-114">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="39bdc-115">managementCondition</span><span class="sxs-lookup"><span data-stu-id="39bdc-115">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="39bdc-116">Leia as propriedades e as relações do objeto [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="39bdc-116">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="39bdc-117">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="39bdc-117">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="39bdc-118">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="39bdc-118">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="39bdc-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="39bdc-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="39bdc-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39bdc-120">Properties</span></span>
|<span data-ttu-id="39bdc-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39bdc-121">Property</span></span>|<span data-ttu-id="39bdc-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="39bdc-122">Type</span></span>|<span data-ttu-id="39bdc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="39bdc-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39bdc-124">id</span><span class="sxs-lookup"><span data-stu-id="39bdc-124">id</span></span>|<span data-ttu-id="39bdc-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39bdc-125">String</span></span>|<span data-ttu-id="39bdc-126">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="39bdc-126">Unique identifier for the management condition.</span></span> <span data-ttu-id="39bdc-127">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="39bdc-127">System generated value assigned when created.</span></span>|
|<span data-ttu-id="39bdc-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="39bdc-128">uniqueName</span></span>|<span data-ttu-id="39bdc-129">String</span><span class="sxs-lookup"><span data-stu-id="39bdc-129">String</span></span>|<span data-ttu-id="39bdc-130">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="39bdc-130">Unique name for the management condition.</span></span> <span data-ttu-id="39bdc-131">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="39bdc-131">Used in management condition expressions.</span></span>|
|<span data-ttu-id="39bdc-132">displayName</span><span class="sxs-lookup"><span data-stu-id="39bdc-132">displayName</span></span>|<span data-ttu-id="39bdc-133">String</span><span class="sxs-lookup"><span data-stu-id="39bdc-133">String</span></span>|<span data-ttu-id="39bdc-134">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="39bdc-134">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="39bdc-135">descrição</span><span class="sxs-lookup"><span data-stu-id="39bdc-135">description</span></span>|<span data-ttu-id="39bdc-136">String</span><span class="sxs-lookup"><span data-stu-id="39bdc-136">String</span></span>|<span data-ttu-id="39bdc-137">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="39bdc-137">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="39bdc-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39bdc-138">createdDateTime</span></span>|<span data-ttu-id="39bdc-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39bdc-139">DateTimeOffset</span></span>|<span data-ttu-id="39bdc-140">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="39bdc-140">The time the management condition was created.</span></span> <span data-ttu-id="39bdc-141">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="39bdc-141">Generated service side.</span></span>|
|<span data-ttu-id="39bdc-142">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39bdc-142">modifiedDateTime</span></span>|<span data-ttu-id="39bdc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39bdc-143">DateTimeOffset</span></span>|<span data-ttu-id="39bdc-144">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="39bdc-144">The time the management condition was last modified.</span></span> <span data-ttu-id="39bdc-145">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="39bdc-145">Updated service side.</span></span>|
|<span data-ttu-id="39bdc-146">eTag</span><span class="sxs-lookup"><span data-stu-id="39bdc-146">eTag</span></span>|<span data-ttu-id="39bdc-147">String</span><span class="sxs-lookup"><span data-stu-id="39bdc-147">String</span></span>|<span data-ttu-id="39bdc-148">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="39bdc-148">ETag of the management condition.</span></span> <span data-ttu-id="39bdc-149">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="39bdc-149">Updated service side.</span></span>|
|<span data-ttu-id="39bdc-150">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="39bdc-150">applicablePlatforms</span></span>|<span data-ttu-id="39bdc-151">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="39bdc-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="39bdc-152">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="39bdc-152">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39bdc-153">Relações</span><span class="sxs-lookup"><span data-stu-id="39bdc-153">Relationships</span></span>
|<span data-ttu-id="39bdc-154">Relação</span><span class="sxs-lookup"><span data-stu-id="39bdc-154">Relationship</span></span>|<span data-ttu-id="39bdc-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="39bdc-155">Type</span></span>|<span data-ttu-id="39bdc-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="39bdc-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39bdc-157">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="39bdc-157">managementConditionStatements</span></span>|<span data-ttu-id="39bdc-158">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="39bdc-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="39bdc-159">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="39bdc-159">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39bdc-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39bdc-160">JSON Representation</span></span>
<span data-ttu-id="39bdc-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39bdc-161">Here is a JSON representation of the resource.</span></span>
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



