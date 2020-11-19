---
title: tipo de recurso deviceComplianceScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 235d5010db7d2235689e51d261e443324cb9a040
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267632"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a><span data-ttu-id="02006-103">tipo de recurso deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="02006-103">deviceComplianceScriptRunSummary resource type</span></span>

<span data-ttu-id="02006-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02006-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02006-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02006-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02006-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02006-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02006-107">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02006-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="02006-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="02006-108">Methods</span></span>
|<span data-ttu-id="02006-109">Método</span><span class="sxs-lookup"><span data-stu-id="02006-109">Method</span></span>|<span data-ttu-id="02006-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="02006-110">Return Type</span></span>|<span data-ttu-id="02006-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="02006-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="02006-112">Obter deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="02006-112">Get deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[<span data-ttu-id="02006-113">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="02006-113">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="02006-114">Leia as propriedades e as relações do objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="02006-114">Read properties and relationships of the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="02006-115">Atualizar deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="02006-115">Update deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[<span data-ttu-id="02006-116">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="02006-116">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="02006-117">Atualiza as propriedades de um objeto [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="02006-117">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="02006-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02006-118">Properties</span></span>
|<span data-ttu-id="02006-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02006-119">Property</span></span>|<span data-ttu-id="02006-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="02006-120">Type</span></span>|<span data-ttu-id="02006-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="02006-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02006-122">id</span><span class="sxs-lookup"><span data-stu-id="02006-122">id</span></span>|<span data-ttu-id="02006-123">String</span><span class="sxs-lookup"><span data-stu-id="02006-123">String</span></span>|<span data-ttu-id="02006-124">Chave da entidade de Resumo de execução de script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02006-124">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="02006-125">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="02006-125">This property is read-only.</span></span>|
|<span data-ttu-id="02006-126">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02006-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="02006-127">Int32</span><span class="sxs-lookup"><span data-stu-id="02006-127">Int32</span></span>|<span data-ttu-id="02006-128">Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está íntegro.</span><span class="sxs-lookup"><span data-stu-id="02006-128">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="02006-129">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="02006-129">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="02006-130">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02006-130">issueDetectedDeviceCount</span></span>|<span data-ttu-id="02006-131">Int32</span><span class="sxs-lookup"><span data-stu-id="02006-131">Int32</span></span>|<span data-ttu-id="02006-132">Número de dispositivos para os quais o script de detecção encontrou um problema.</span><span class="sxs-lookup"><span data-stu-id="02006-132">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="02006-133">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="02006-133">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="02006-134">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02006-134">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="02006-135">Int32</span><span class="sxs-lookup"><span data-stu-id="02006-135">Int32</span></span>|<span data-ttu-id="02006-136">Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída.</span><span class="sxs-lookup"><span data-stu-id="02006-136">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="02006-137">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="02006-137">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="02006-138">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02006-138">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="02006-139">Int32</span><span class="sxs-lookup"><span data-stu-id="02006-139">Int32</span></span>|<span data-ttu-id="02006-140">Número de dispositivos que ainda não executaram a versão mais recente do script de conformidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02006-140">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="02006-141">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="02006-141">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="02006-142">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="02006-142">lastScriptRunDateTime</span></span>|<span data-ttu-id="02006-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02006-143">DateTimeOffset</span></span>|<span data-ttu-id="02006-144">Hora da última execução para o script em todos os dispositivos</span><span class="sxs-lookup"><span data-stu-id="02006-144">Last run time for the script across all devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="02006-145">Relações</span><span class="sxs-lookup"><span data-stu-id="02006-145">Relationships</span></span>
<span data-ttu-id="02006-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="02006-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02006-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02006-147">JSON Representation</span></span>
<span data-ttu-id="02006-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02006-148">Here is a JSON representation of the resource.</span></span>
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




