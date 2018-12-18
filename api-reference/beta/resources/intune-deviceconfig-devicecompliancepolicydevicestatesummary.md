---
title: Tipo de recurso deviceCompliancePolicyDeviceStateSummary
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 006b1ca71f8441898ba758397334c7ae31ac5690
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318806"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a><span data-ttu-id="05872-103">Tipo de recurso deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="05872-103">deviceCompliancePolicyDeviceStateSummary resource type</span></span>

> <span data-ttu-id="05872-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="05872-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05872-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="05872-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05872-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="05872-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05872-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="05872-107">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="05872-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="05872-108">Methods</span></span>
|<span data-ttu-id="05872-109">Método</span><span class="sxs-lookup"><span data-stu-id="05872-109">Method</span></span>|<span data-ttu-id="05872-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="05872-110">Return Type</span></span>|<span data-ttu-id="05872-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="05872-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05872-112">Obter deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="05872-112">Get deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[<span data-ttu-id="05872-113">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="05872-113">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="05872-114">Ler propriedades e relações de objetos de [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="05872-114">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="05872-115">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="05872-115">Update deviceCompliancePolicyDeviceStateSummary</span></span>](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[<span data-ttu-id="05872-116">deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="05872-116">deviceCompliancePolicyDeviceStateSummary</span></span>](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|<span data-ttu-id="05872-117">Atualizar as propriedades de um objeto de [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="05872-117">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="05872-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05872-118">Properties</span></span>
|<span data-ttu-id="05872-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05872-119">Property</span></span>|<span data-ttu-id="05872-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="05872-120">Type</span></span>|<span data-ttu-id="05872-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="05872-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05872-122">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="05872-122">inGracePeriodCount</span></span>|<span data-ttu-id="05872-123">Int32</span><span class="sxs-lookup"><span data-stu-id="05872-123">Int32</span></span>|<span data-ttu-id="05872-124">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="05872-124">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="05872-125">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="05872-125">configManagerCount</span></span>|<span data-ttu-id="05872-126">Int32</span><span class="sxs-lookup"><span data-stu-id="05872-126">Int32</span></span>|<span data-ttu-id="05872-127">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="05872-127">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="05872-128">id</span><span class="sxs-lookup"><span data-stu-id="05872-128">id</span></span>|<span data-ttu-id="05872-129">String</span><span class="sxs-lookup"><span data-stu-id="05872-129">String</span></span>|<span data-ttu-id="05872-130">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05872-130">Key of the entity.</span></span>|
|<span data-ttu-id="05872-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05872-131">unknownDeviceCount</span></span>|<span data-ttu-id="05872-132">Int32</span><span class="sxs-lookup"><span data-stu-id="05872-132">Int32</span></span>|<span data-ttu-id="05872-133">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="05872-133">Number of unknown devices</span></span>|
|<span data-ttu-id="05872-134">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05872-134">notApplicableDeviceCount</span></span>|<span data-ttu-id="05872-135">Int32</span><span class="sxs-lookup"><span data-stu-id="05872-135">Int32</span></span>|<span data-ttu-id="05872-136">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="05872-136">Number of not applicable devices</span></span>|
|<span data-ttu-id="05872-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05872-137">compliantDeviceCount</span></span>|<span data-ttu-id="05872-138">Int32</span><span class="sxs-lookup"><span data-stu-id="05872-138">Int32</span></span>|<span data-ttu-id="05872-139">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="05872-139">Number of compliant devices</span></span>|
|<span data-ttu-id="05872-140">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05872-140">remediatedDeviceCount</span></span>|<span data-ttu-id="05872-141">Int32</span><span class="sxs-lookup"><span data-stu-id="05872-141">Int32</span></span>|<span data-ttu-id="05872-142">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="05872-142">Number of remediated devices</span></span>|
|<span data-ttu-id="05872-143">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05872-143">nonCompliantDeviceCount</span></span>|<span data-ttu-id="05872-144">Int32</span><span class="sxs-lookup"><span data-stu-id="05872-144">Int32</span></span>|<span data-ttu-id="05872-145">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="05872-145">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="05872-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05872-146">errorDeviceCount</span></span>|<span data-ttu-id="05872-147">Int32</span><span class="sxs-lookup"><span data-stu-id="05872-147">Int32</span></span>|<span data-ttu-id="05872-148">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="05872-148">Number of error devices</span></span>|
|<span data-ttu-id="05872-149">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05872-149">conflictDeviceCount</span></span>|<span data-ttu-id="05872-150">Int32</span><span class="sxs-lookup"><span data-stu-id="05872-150">Int32</span></span>|<span data-ttu-id="05872-151">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="05872-151">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="05872-152">Relações</span><span class="sxs-lookup"><span data-stu-id="05872-152">Relationships</span></span>
<span data-ttu-id="05872-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05872-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="05872-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05872-154">JSON Representation</span></span>
<span data-ttu-id="05872-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05872-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





