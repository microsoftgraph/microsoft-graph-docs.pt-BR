---
title: tipo de recurso de managementCondition
description: Condições de gerenciamento são eventos que podem ser disparados dinamicamente como limites de geo, limites de tempo e limites de rede.
ms.openlocfilehash: 3c2bc1d7594e61642b96398bfb55d6aa38f3283d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035173"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="cd2ab-103">tipo de recurso de managementCondition</span><span class="sxs-lookup"><span data-stu-id="cd2ab-103">managementCondition resource type</span></span>

> <span data-ttu-id="cd2ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd2ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd2ab-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd2ab-107">Condições de gerenciamento são eventos que podem ser disparados dinamicamente como limites de geo, limites de tempo e limites de rede.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>
## <a name="methods"></a><span data-ttu-id="cd2ab-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="cd2ab-108">Methods</span></span>
|<span data-ttu-id="cd2ab-109">Método</span><span class="sxs-lookup"><span data-stu-id="cd2ab-109">Method</span></span>|<span data-ttu-id="cd2ab-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd2ab-110">Return Type</span></span>|<span data-ttu-id="cd2ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2ab-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cd2ab-112">Lista managementConditions</span><span class="sxs-lookup"><span data-stu-id="cd2ab-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="cd2ab-113">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cd2ab-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="cd2ab-114">Lista as propriedades e os relacionamentos dos objetos [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cd2ab-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="cd2ab-115">Obter managementCondition</span><span class="sxs-lookup"><span data-stu-id="cd2ab-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="cd2ab-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="cd2ab-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="cd2ab-117">Leia as propriedades e os relacionamentos do objeto [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cd2ab-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="cd2ab-118">função getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="cd2ab-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="cd2ab-119">coleção [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cd2ab-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="cd2ab-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cd2ab-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cd2ab-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd2ab-121">Properties</span></span>
|<span data-ttu-id="cd2ab-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd2ab-122">Property</span></span>|<span data-ttu-id="cd2ab-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd2ab-123">Type</span></span>|<span data-ttu-id="cd2ab-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2ab-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd2ab-125">id</span><span class="sxs-lookup"><span data-stu-id="cd2ab-125">id</span></span>|<span data-ttu-id="cd2ab-126">String</span><span class="sxs-lookup"><span data-stu-id="cd2ab-126">String</span></span>|<span data-ttu-id="cd2ab-127">Identificador exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="cd2ab-128">Valor atribuído quando criado gerado pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="cd2ab-129">nome exclusivo</span><span class="sxs-lookup"><span data-stu-id="cd2ab-129">uniqueName</span></span>|<span data-ttu-id="cd2ab-130">String</span><span class="sxs-lookup"><span data-stu-id="cd2ab-130">String</span></span>|<span data-ttu-id="cd2ab-131">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-131">Unique name for the management condition.</span></span> <span data-ttu-id="cd2ab-132">Usadas nas expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="cd2ab-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cd2ab-133">displayName</span></span>|<span data-ttu-id="cd2ab-134">String</span><span class="sxs-lookup"><span data-stu-id="cd2ab-134">String</span></span>|<span data-ttu-id="cd2ab-135">O nome definido admin da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="cd2ab-136">description</span><span class="sxs-lookup"><span data-stu-id="cd2ab-136">description</span></span>|<span data-ttu-id="cd2ab-137">String</span><span class="sxs-lookup"><span data-stu-id="cd2ab-137">String</span></span>|<span data-ttu-id="cd2ab-138">O administrador definidos descrição da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="cd2ab-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd2ab-139">createdDateTime</span></span>|<span data-ttu-id="cd2ab-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd2ab-140">DateTimeOffset</span></span>|<span data-ttu-id="cd2ab-141">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-141">The time the management condition was created.</span></span> <span data-ttu-id="cd2ab-142">Lado de serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-142">Generated service side.</span></span>|
|<span data-ttu-id="cd2ab-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd2ab-143">modifiedDateTime</span></span>|<span data-ttu-id="cd2ab-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd2ab-144">DateTimeOffset</span></span>|<span data-ttu-id="cd2ab-145">A hora que da última modificação a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-145">The time the management condition was last modified.</span></span> <span data-ttu-id="cd2ab-146">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-146">Updated service side.</span></span>|
|<span data-ttu-id="cd2ab-147">eTag</span><span class="sxs-lookup"><span data-stu-id="cd2ab-147">eTag</span></span>|<span data-ttu-id="cd2ab-148">String</span><span class="sxs-lookup"><span data-stu-id="cd2ab-148">String</span></span>|<span data-ttu-id="cd2ab-149">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-149">ETag of the management condition.</span></span> <span data-ttu-id="cd2ab-150">Lado de serviços atualizado.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-150">Updated service side.</span></span>|
|<span data-ttu-id="cd2ab-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="cd2ab-151">applicablePlatforms</span></span>|<span data-ttu-id="cd2ab-152">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="cd2ab-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="cd2ab-153">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd2ab-154">Relações</span><span class="sxs-lookup"><span data-stu-id="cd2ab-154">Relationships</span></span>
|<span data-ttu-id="cd2ab-155">Relação</span><span class="sxs-lookup"><span data-stu-id="cd2ab-155">Relationship</span></span>|<span data-ttu-id="cd2ab-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd2ab-156">Type</span></span>|<span data-ttu-id="cd2ab-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2ab-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd2ab-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="cd2ab-158">managementConditionStatements</span></span>|<span data-ttu-id="cd2ab-159">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="cd2ab-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="cd2ab-160">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd2ab-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd2ab-161">JSON Representation</span></span>
<span data-ttu-id="cd2ab-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd2ab-162">Here is a JSON representation of the resource.</span></span>
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





