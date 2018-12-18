---
title: Tipo de recurso settingStateDeviceSummary
description: Configuração e política de conformidade de dispositivo para um resumo de estado de configuração
author: tfitzmac
ms.openlocfilehash: dff6f8966d321aa706fceabceb14a418ae8433f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318533"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="65713-103">Tipo de recurso settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="65713-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="65713-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="65713-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65713-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="65713-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65713-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="65713-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65713-107">Configuração e política de conformidade de dispositivo para um resumo de estado de configuração</span><span class="sxs-lookup"><span data-stu-id="65713-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>
## <a name="methods"></a><span data-ttu-id="65713-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="65713-108">Methods</span></span>
|<span data-ttu-id="65713-109">Método</span><span class="sxs-lookup"><span data-stu-id="65713-109">Method</span></span>|<span data-ttu-id="65713-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="65713-110">Return Type</span></span>|<span data-ttu-id="65713-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="65713-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="65713-112">Listar settingStateDeviceSummaries</span><span class="sxs-lookup"><span data-stu-id="65713-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="65713-113">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="65713-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="65713-114">Listar propriedades e relações de objetos de [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="65713-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="65713-115">Obter settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="65713-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="65713-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="65713-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="65713-117">Ler propriedades e relações de objetos de [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="65713-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="65713-118">Criar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="65713-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="65713-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="65713-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="65713-120">Criar um novo objeto de [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="65713-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="65713-121">Excluir settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="65713-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="65713-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65713-122">None</span></span>|<span data-ttu-id="65713-123">Excluir [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="65713-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="65713-124">Atualizar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="65713-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="65713-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="65713-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="65713-126">Atualizar as propriedades de um objeto de [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="65713-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="65713-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65713-127">Properties</span></span>
|<span data-ttu-id="65713-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65713-128">Property</span></span>|<span data-ttu-id="65713-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="65713-129">Type</span></span>|<span data-ttu-id="65713-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="65713-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65713-131">id</span><span class="sxs-lookup"><span data-stu-id="65713-131">id</span></span>|<span data-ttu-id="65713-132">String</span><span class="sxs-lookup"><span data-stu-id="65713-132">String</span></span>|<span data-ttu-id="65713-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="65713-133">Key of the entity.</span></span>|
|<span data-ttu-id="65713-134">settingName</span><span class="sxs-lookup"><span data-stu-id="65713-134">settingName</span></span>|<span data-ttu-id="65713-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65713-135">String</span></span>|<span data-ttu-id="65713-136">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="65713-136">Name of the setting</span></span>|
|<span data-ttu-id="65713-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="65713-137">instancePath</span></span>|<span data-ttu-id="65713-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65713-138">String</span></span>|<span data-ttu-id="65713-139">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="65713-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="65713-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65713-140">unknownDeviceCount</span></span>|<span data-ttu-id="65713-141">Int32</span><span class="sxs-lookup"><span data-stu-id="65713-141">Int32</span></span>|<span data-ttu-id="65713-142">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="65713-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="65713-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65713-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="65713-144">Int32</span><span class="sxs-lookup"><span data-stu-id="65713-144">Int32</span></span>|<span data-ttu-id="65713-145">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="65713-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="65713-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65713-146">compliantDeviceCount</span></span>|<span data-ttu-id="65713-147">Int32</span><span class="sxs-lookup"><span data-stu-id="65713-147">Int32</span></span>|<span data-ttu-id="65713-148">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="65713-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="65713-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65713-149">remediatedDeviceCount</span></span>|<span data-ttu-id="65713-150">Int32</span><span class="sxs-lookup"><span data-stu-id="65713-150">Int32</span></span>|<span data-ttu-id="65713-151">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="65713-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="65713-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65713-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="65713-153">Int32</span><span class="sxs-lookup"><span data-stu-id="65713-153">Int32</span></span>|<span data-ttu-id="65713-154">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="65713-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="65713-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65713-155">errorDeviceCount</span></span>|<span data-ttu-id="65713-156">Int32</span><span class="sxs-lookup"><span data-stu-id="65713-156">Int32</span></span>|<span data-ttu-id="65713-157">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="65713-157">Device error count for the setting</span></span>|
|<span data-ttu-id="65713-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65713-158">conflictDeviceCount</span></span>|<span data-ttu-id="65713-159">Int32</span><span class="sxs-lookup"><span data-stu-id="65713-159">Int32</span></span>|<span data-ttu-id="65713-160">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="65713-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="65713-161">Relações</span><span class="sxs-lookup"><span data-stu-id="65713-161">Relationships</span></span>
<span data-ttu-id="65713-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65713-162">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65713-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65713-163">JSON Representation</span></span>
<span data-ttu-id="65713-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65713-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





