---
title: tipo de recurso deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9d2b0b92287a045607c02e271155e2e74a2fa90
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370022"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="c7d43-103">tipo de recurso deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c7d43-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="c7d43-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7d43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7d43-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7d43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7d43-106">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7d43-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="c7d43-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c7d43-107">Methods</span></span>
|<span data-ttu-id="c7d43-108">Método</span><span class="sxs-lookup"><span data-stu-id="c7d43-108">Method</span></span>|<span data-ttu-id="c7d43-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c7d43-109">Return Type</span></span>|<span data-ttu-id="c7d43-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7d43-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7d43-111">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c7d43-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="c7d43-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c7d43-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="c7d43-113">Leia as propriedades e as relações do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c7d43-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="c7d43-114">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c7d43-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="c7d43-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c7d43-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="c7d43-116">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c7d43-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7d43-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7d43-117">Properties</span></span>
|<span data-ttu-id="c7d43-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7d43-118">Property</span></span>|<span data-ttu-id="c7d43-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7d43-119">Type</span></span>|<span data-ttu-id="c7d43-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7d43-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7d43-121">id</span><span class="sxs-lookup"><span data-stu-id="c7d43-121">id</span></span>|<span data-ttu-id="c7d43-122">String</span><span class="sxs-lookup"><span data-stu-id="c7d43-122">String</span></span>|<span data-ttu-id="c7d43-123">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7d43-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="c7d43-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7d43-124">successDeviceCount</span></span>|<span data-ttu-id="c7d43-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d43-125">Int32</span></span>|<span data-ttu-id="c7d43-126">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="c7d43-126">Success device count.</span></span>|
|<span data-ttu-id="c7d43-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7d43-127">errorDeviceCount</span></span>|<span data-ttu-id="c7d43-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d43-128">Int32</span></span>|<span data-ttu-id="c7d43-129">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="c7d43-129">Error device count.</span></span>|
|<span data-ttu-id="c7d43-130">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7d43-130">compliantDeviceCount</span></span>|<span data-ttu-id="c7d43-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d43-131">Int32</span></span>|<span data-ttu-id="c7d43-132">Contagem de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="c7d43-132">Compliant device count.</span></span>|
|<span data-ttu-id="c7d43-133">notCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7d43-133">notCompliantDeviceCount</span></span>|<span data-ttu-id="c7d43-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d43-134">Int32</span></span>|<span data-ttu-id="c7d43-135">Contagem de dispositivos não compatíveis.</span><span class="sxs-lookup"><span data-stu-id="c7d43-135">Not Compliant device count.</span></span>|
|<span data-ttu-id="c7d43-136">pendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c7d43-136">pendingDeviceCount</span></span>|<span data-ttu-id="c7d43-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d43-137">Int32</span></span>|<span data-ttu-id="c7d43-138">Contagem de dispositivos pendentes.</span><span class="sxs-lookup"><span data-stu-id="c7d43-138">Pending device count.</span></span>|
|<span data-ttu-id="c7d43-139">successUserCount</span><span class="sxs-lookup"><span data-stu-id="c7d43-139">successUserCount</span></span>|<span data-ttu-id="c7d43-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d43-140">Int32</span></span>|<span data-ttu-id="c7d43-141">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="c7d43-141">Success user count.</span></span>|
|<span data-ttu-id="c7d43-142">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="c7d43-142">errorUserCount</span></span>|<span data-ttu-id="c7d43-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c7d43-143">Int32</span></span>|<span data-ttu-id="c7d43-144">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="c7d43-144">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7d43-145">Relações</span><span class="sxs-lookup"><span data-stu-id="c7d43-145">Relationships</span></span>
<span data-ttu-id="c7d43-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7d43-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7d43-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7d43-147">JSON Representation</span></span>
<span data-ttu-id="c7d43-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7d43-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "notCompliantDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```



