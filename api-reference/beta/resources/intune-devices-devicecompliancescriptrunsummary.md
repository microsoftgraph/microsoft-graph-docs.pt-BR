---
title: tipo de recurso deviceComplianceScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c436261961be8938e8905bc9f19be1690c7f79c4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789307"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a><span data-ttu-id="79fba-103">tipo de recurso deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="79fba-103">deviceComplianceScriptRunSummary resource type</span></span>

<span data-ttu-id="79fba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79fba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79fba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79fba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79fba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79fba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79fba-107">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79fba-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="79fba-108">Methods</span><span class="sxs-lookup"><span data-stu-id="79fba-108">Methods</span></span>
|<span data-ttu-id="79fba-109">Método</span><span class="sxs-lookup"><span data-stu-id="79fba-109">Method</span></span>|<span data-ttu-id="79fba-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="79fba-110">Return Type</span></span>|<span data-ttu-id="79fba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="79fba-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="79fba-112">Obter deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="79fba-112">Get deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[<span data-ttu-id="79fba-113">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="79fba-113">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="79fba-114">Leia as propriedades e as relações do objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="79fba-114">Read properties and relationships of the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="79fba-115">Atualizar deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="79fba-115">Update deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[<span data-ttu-id="79fba-116">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="79fba-116">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="79fba-117">Atualiza as propriedades de um objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="79fba-117">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="79fba-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79fba-118">Properties</span></span>
|<span data-ttu-id="79fba-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79fba-119">Property</span></span>|<span data-ttu-id="79fba-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="79fba-120">Type</span></span>|<span data-ttu-id="79fba-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="79fba-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79fba-122">id</span><span class="sxs-lookup"><span data-stu-id="79fba-122">id</span></span>|<span data-ttu-id="79fba-123">String</span><span class="sxs-lookup"><span data-stu-id="79fba-123">String</span></span>|<span data-ttu-id="79fba-124">Chave da entidade de Resumo de execução de script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79fba-124">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="79fba-125">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79fba-125">This property is read-only.</span></span>|
|<span data-ttu-id="79fba-126">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79fba-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="79fba-127">Int32</span><span class="sxs-lookup"><span data-stu-id="79fba-127">Int32</span></span>|<span data-ttu-id="79fba-128">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro.</span><span class="sxs-lookup"><span data-stu-id="79fba-128">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="79fba-129">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="79fba-129">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="79fba-130">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79fba-130">issueDetectedDeviceCount</span></span>|<span data-ttu-id="79fba-131">Int32</span><span class="sxs-lookup"><span data-stu-id="79fba-131">Int32</span></span>|<span data-ttu-id="79fba-132">Número de dispositivos para os quais o script de detecção encontrou um problema.</span><span class="sxs-lookup"><span data-stu-id="79fba-132">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="79fba-133">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="79fba-133">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="79fba-134">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79fba-134">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="79fba-135">Int32</span><span class="sxs-lookup"><span data-stu-id="79fba-135">Int32</span></span>|<span data-ttu-id="79fba-136">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída.</span><span class="sxs-lookup"><span data-stu-id="79fba-136">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="79fba-137">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="79fba-137">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="79fba-138">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="79fba-138">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="79fba-139">Int32</span><span class="sxs-lookup"><span data-stu-id="79fba-139">Int32</span></span>|<span data-ttu-id="79fba-140">Número de dispositivos que ainda não executaram a versão mais recente do script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79fba-140">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="79fba-141">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="79fba-141">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="79fba-142">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="79fba-142">lastScriptRunDateTime</span></span>|<span data-ttu-id="79fba-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79fba-143">DateTimeOffset</span></span>|<span data-ttu-id="79fba-144">Hora da última execução para o script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="79fba-144">Last run time for the script across all devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="79fba-145">Relações</span><span class="sxs-lookup"><span data-stu-id="79fba-145">Relationships</span></span>
<span data-ttu-id="79fba-146">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="79fba-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79fba-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79fba-147">JSON Representation</span></span>
<span data-ttu-id="79fba-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79fba-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)"
}
```



