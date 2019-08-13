---
title: tipo de recurso networkManagementCondition
description: Contém as informações para definir uma condição de gerenciamento de rede.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7328f061ab459fd02c088e403c7c46a3bc827c60
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331585"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="970b6-103">tipo de recurso networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="970b6-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="970b6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="970b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="970b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="970b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="970b6-106">Contém as informações para definir uma condição de gerenciamento de rede.</span><span class="sxs-lookup"><span data-stu-id="970b6-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="970b6-107">Herda de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="970b6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="970b6-108">Methods</span></span>
|<span data-ttu-id="970b6-109">Método</span><span class="sxs-lookup"><span data-stu-id="970b6-109">Method</span></span>|<span data-ttu-id="970b6-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="970b6-110">Return Type</span></span>|<span data-ttu-id="970b6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="970b6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="970b6-112">Listar networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="970b6-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="970b6-113">coleção [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="970b6-114">Listar Propriedades e relações dos objetos [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="970b6-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="970b6-115">Obter networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="970b6-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="970b6-116">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="970b6-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="970b6-117">Leia as propriedades e as relações do objeto [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="970b6-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="970b6-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="970b6-118">Properties</span></span>
|<span data-ttu-id="970b6-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="970b6-119">Property</span></span>|<span data-ttu-id="970b6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="970b6-120">Type</span></span>|<span data-ttu-id="970b6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="970b6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="970b6-122">id</span><span class="sxs-lookup"><span data-stu-id="970b6-122">id</span></span>|<span data-ttu-id="970b6-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="970b6-123">String</span></span>|<span data-ttu-id="970b6-124">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="970b6-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="970b6-125">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="970b6-125">System generated value assigned when created.</span></span> <span data-ttu-id="970b6-126">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="970b6-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="970b6-127">uniqueName</span></span>|<span data-ttu-id="970b6-128">String</span><span class="sxs-lookup"><span data-stu-id="970b6-128">String</span></span>|<span data-ttu-id="970b6-129">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="970b6-129">Unique name for the management condition.</span></span> <span data-ttu-id="970b6-130">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="970b6-130">Used in management condition expressions.</span></span> <span data-ttu-id="970b6-131">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="970b6-132">displayName</span><span class="sxs-lookup"><span data-stu-id="970b6-132">displayName</span></span>|<span data-ttu-id="970b6-133">String</span><span class="sxs-lookup"><span data-stu-id="970b6-133">String</span></span>|<span data-ttu-id="970b6-134">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="970b6-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="970b6-135">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="970b6-136">descrição</span><span class="sxs-lookup"><span data-stu-id="970b6-136">description</span></span>|<span data-ttu-id="970b6-137">String</span><span class="sxs-lookup"><span data-stu-id="970b6-137">String</span></span>|<span data-ttu-id="970b6-138">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="970b6-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="970b6-139">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="970b6-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="970b6-140">createdDateTime</span></span>|<span data-ttu-id="970b6-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="970b6-141">DateTimeOffset</span></span>|<span data-ttu-id="970b6-142">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="970b6-142">The time the management condition was created.</span></span> <span data-ttu-id="970b6-143">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="970b6-143">Generated service side.</span></span> <span data-ttu-id="970b6-144">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="970b6-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="970b6-145">modifiedDateTime</span></span>|<span data-ttu-id="970b6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="970b6-146">DateTimeOffset</span></span>|<span data-ttu-id="970b6-147">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="970b6-147">The time the management condition was last modified.</span></span> <span data-ttu-id="970b6-148">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="970b6-148">Updated service side.</span></span> <span data-ttu-id="970b6-149">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="970b6-150">eTag</span><span class="sxs-lookup"><span data-stu-id="970b6-150">eTag</span></span>|<span data-ttu-id="970b6-151">String</span><span class="sxs-lookup"><span data-stu-id="970b6-151">String</span></span>|<span data-ttu-id="970b6-152">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="970b6-152">ETag of the management condition.</span></span> <span data-ttu-id="970b6-153">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="970b6-153">Updated service side.</span></span> <span data-ttu-id="970b6-154">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="970b6-155">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="970b6-155">applicablePlatforms</span></span>|<span data-ttu-id="970b6-156">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="970b6-157">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="970b6-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="970b6-158">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="970b6-159">Relações</span><span class="sxs-lookup"><span data-stu-id="970b6-159">Relationships</span></span>
|<span data-ttu-id="970b6-160">Relação</span><span class="sxs-lookup"><span data-stu-id="970b6-160">Relationship</span></span>|<span data-ttu-id="970b6-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="970b6-161">Type</span></span>|<span data-ttu-id="970b6-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="970b6-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="970b6-163">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="970b6-163">managementConditionStatements</span></span>|<span data-ttu-id="970b6-164">coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="970b6-165">As instruções de condição de gerenciamento associadas à condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="970b6-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="970b6-166">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="970b6-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="970b6-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="970b6-167">JSON Representation</span></span>
<span data-ttu-id="970b6-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="970b6-168">Here is a JSON representation of the resource.</span></span>
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



