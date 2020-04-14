---
title: tipo de recurso managementCondition
description: As condições de gerenciamento são eventos que podem ser acionados dinamicamente, como isolamentos geográficos, cercas de tempo e cercas de rede.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24aca3452d6dcb6dd43290c8ce2359551db65331
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382649"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="03bfc-103">tipo de recurso managementCondition</span><span class="sxs-lookup"><span data-stu-id="03bfc-103">managementCondition resource type</span></span>

<span data-ttu-id="03bfc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03bfc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03bfc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03bfc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03bfc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03bfc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03bfc-107">As condições de gerenciamento são eventos que podem ser acionados dinamicamente, como isolamentos geográficos, cercas de tempo e cercas de rede.</span><span class="sxs-lookup"><span data-stu-id="03bfc-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="03bfc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="03bfc-108">Methods</span></span>
|<span data-ttu-id="03bfc-109">Método</span><span class="sxs-lookup"><span data-stu-id="03bfc-109">Method</span></span>|<span data-ttu-id="03bfc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03bfc-110">Return Type</span></span>|<span data-ttu-id="03bfc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="03bfc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03bfc-112">Listar managementConditions</span><span class="sxs-lookup"><span data-stu-id="03bfc-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="03bfc-113">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="03bfc-114">Listar Propriedades e relações dos objetos [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="03bfc-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="03bfc-115">Obter managementCondition</span><span class="sxs-lookup"><span data-stu-id="03bfc-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="03bfc-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="03bfc-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="03bfc-117">Leia as propriedades e as relações do objeto [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="03bfc-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="03bfc-118">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="03bfc-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="03bfc-119">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="03bfc-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="03bfc-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="03bfc-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03bfc-121">Properties</span></span>
|<span data-ttu-id="03bfc-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03bfc-122">Property</span></span>|<span data-ttu-id="03bfc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="03bfc-123">Type</span></span>|<span data-ttu-id="03bfc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="03bfc-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03bfc-125">id</span><span class="sxs-lookup"><span data-stu-id="03bfc-125">id</span></span>|<span data-ttu-id="03bfc-126">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-126">String</span></span>|<span data-ttu-id="03bfc-127">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="03bfc-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="03bfc-128">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="03bfc-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="03bfc-129">uniqueName</span><span class="sxs-lookup"><span data-stu-id="03bfc-129">uniqueName</span></span>|<span data-ttu-id="03bfc-130">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-130">String</span></span>|<span data-ttu-id="03bfc-131">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="03bfc-131">Unique name for the management condition.</span></span> <span data-ttu-id="03bfc-132">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="03bfc-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="03bfc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="03bfc-133">displayName</span></span>|<span data-ttu-id="03bfc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03bfc-134">String</span></span>|<span data-ttu-id="03bfc-135">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="03bfc-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="03bfc-136">description</span><span class="sxs-lookup"><span data-stu-id="03bfc-136">description</span></span>|<span data-ttu-id="03bfc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03bfc-137">String</span></span>|<span data-ttu-id="03bfc-138">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="03bfc-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="03bfc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03bfc-139">createdDateTime</span></span>|<span data-ttu-id="03bfc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03bfc-140">DateTimeOffset</span></span>|<span data-ttu-id="03bfc-141">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="03bfc-141">The time the management condition was created.</span></span> <span data-ttu-id="03bfc-142">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="03bfc-142">Generated service side.</span></span>|
|<span data-ttu-id="03bfc-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03bfc-143">modifiedDateTime</span></span>|<span data-ttu-id="03bfc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03bfc-144">DateTimeOffset</span></span>|<span data-ttu-id="03bfc-145">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="03bfc-145">The time the management condition was last modified.</span></span> <span data-ttu-id="03bfc-146">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="03bfc-146">Updated service side.</span></span>|
|<span data-ttu-id="03bfc-147">eTag</span><span class="sxs-lookup"><span data-stu-id="03bfc-147">eTag</span></span>|<span data-ttu-id="03bfc-148">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-148">String</span></span>|<span data-ttu-id="03bfc-149">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="03bfc-149">ETag of the management condition.</span></span> <span data-ttu-id="03bfc-150">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="03bfc-150">Updated service side.</span></span>|
|<span data-ttu-id="03bfc-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="03bfc-151">applicablePlatforms</span></span>|<span data-ttu-id="03bfc-152">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="03bfc-153">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="03bfc-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03bfc-154">Relações</span><span class="sxs-lookup"><span data-stu-id="03bfc-154">Relationships</span></span>
|<span data-ttu-id="03bfc-155">Relação</span><span class="sxs-lookup"><span data-stu-id="03bfc-155">Relationship</span></span>|<span data-ttu-id="03bfc-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="03bfc-156">Type</span></span>|<span data-ttu-id="03bfc-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="03bfc-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03bfc-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="03bfc-158">managementConditionStatements</span></span>|<span data-ttu-id="03bfc-159">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="03bfc-160">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="03bfc-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03bfc-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03bfc-161">JSON Representation</span></span>
<span data-ttu-id="03bfc-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03bfc-162">Here is a JSON representation of the resource.</span></span>
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



