---
title: tipo de recurso deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3fe26fc121d0d1d9339de999101975d2c4c225a5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174267"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="d8f4a-103">tipo de recurso deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d8f4a-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="d8f4a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8f4a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8f4a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8f4a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8f4a-106">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8f4a-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="d8f4a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d8f4a-107">Methods</span></span>
|<span data-ttu-id="d8f4a-108">Método</span><span class="sxs-lookup"><span data-stu-id="d8f4a-108">Method</span></span>|<span data-ttu-id="d8f4a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8f4a-109">Return Type</span></span>|<span data-ttu-id="d8f4a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8f4a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8f4a-111">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d8f4a-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="d8f4a-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d8f4a-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="d8f4a-113">Leia as propriedades e as relações do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d8f4a-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="d8f4a-114">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d8f4a-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="d8f4a-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="d8f4a-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="d8f4a-116">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d8f4a-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8f4a-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8f4a-117">Properties</span></span>
|<span data-ttu-id="d8f4a-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8f4a-118">Property</span></span>|<span data-ttu-id="d8f4a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8f4a-119">Type</span></span>|<span data-ttu-id="d8f4a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8f4a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8f4a-121">id</span><span class="sxs-lookup"><span data-stu-id="d8f4a-121">id</span></span>|<span data-ttu-id="d8f4a-122">String</span><span class="sxs-lookup"><span data-stu-id="d8f4a-122">String</span></span>|<span data-ttu-id="d8f4a-123">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8f4a-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="d8f4a-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8f4a-124">successDeviceCount</span></span>|<span data-ttu-id="d8f4a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f4a-125">Int32</span></span>|<span data-ttu-id="d8f4a-126">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="d8f4a-126">Success device count.</span></span>|
|<span data-ttu-id="d8f4a-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8f4a-127">errorDeviceCount</span></span>|<span data-ttu-id="d8f4a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f4a-128">Int32</span></span>|<span data-ttu-id="d8f4a-129">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="d8f4a-129">Error device count.</span></span>|
|<span data-ttu-id="d8f4a-130">successUserCount</span><span class="sxs-lookup"><span data-stu-id="d8f4a-130">successUserCount</span></span>|<span data-ttu-id="d8f4a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f4a-131">Int32</span></span>|<span data-ttu-id="d8f4a-132">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="d8f4a-132">Success user count.</span></span>|
|<span data-ttu-id="d8f4a-133">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="d8f4a-133">errorUserCount</span></span>|<span data-ttu-id="d8f4a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d8f4a-134">Int32</span></span>|<span data-ttu-id="d8f4a-135">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="d8f4a-135">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8f4a-136">Relações</span><span class="sxs-lookup"><span data-stu-id="d8f4a-136">Relationships</span></span>
<span data-ttu-id="d8f4a-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8f4a-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8f4a-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8f4a-138">JSON Representation</span></span>
<span data-ttu-id="d8f4a-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8f4a-139">Here is a JSON representation of the resource.</span></span>
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
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```




