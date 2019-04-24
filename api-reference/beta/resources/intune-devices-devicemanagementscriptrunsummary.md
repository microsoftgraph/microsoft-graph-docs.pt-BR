---
title: tipo de recurso deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6807114ebaf7ba3a778520c7b2a383f5a13c31f1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522444"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="4c21e-103">tipo de recurso deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="4c21e-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="4c21e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c21e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c21e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c21e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c21e-106">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c21e-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="4c21e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4c21e-107">Methods</span></span>
|<span data-ttu-id="4c21e-108">Método</span><span class="sxs-lookup"><span data-stu-id="4c21e-108">Method</span></span>|<span data-ttu-id="4c21e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4c21e-109">Return Type</span></span>|<span data-ttu-id="4c21e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c21e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4c21e-111">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="4c21e-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="4c21e-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="4c21e-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="4c21e-113">Leia as propriedades e as relações do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4c21e-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="4c21e-114">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="4c21e-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="4c21e-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="4c21e-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="4c21e-116">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4c21e-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c21e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c21e-117">Properties</span></span>
|<span data-ttu-id="4c21e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c21e-118">Property</span></span>|<span data-ttu-id="4c21e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c21e-119">Type</span></span>|<span data-ttu-id="4c21e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c21e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c21e-121">id</span><span class="sxs-lookup"><span data-stu-id="4c21e-121">id</span></span>|<span data-ttu-id="4c21e-122">String</span><span class="sxs-lookup"><span data-stu-id="4c21e-122">String</span></span>|<span data-ttu-id="4c21e-123">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c21e-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="4c21e-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c21e-124">successDeviceCount</span></span>|<span data-ttu-id="4c21e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4c21e-125">Int32</span></span>|<span data-ttu-id="4c21e-126">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="4c21e-126">Success device count.</span></span>|
|<span data-ttu-id="4c21e-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c21e-127">errorDeviceCount</span></span>|<span data-ttu-id="4c21e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="4c21e-128">Int32</span></span>|<span data-ttu-id="4c21e-129">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="4c21e-129">Error device count.</span></span>|
|<span data-ttu-id="4c21e-130">successUserCount</span><span class="sxs-lookup"><span data-stu-id="4c21e-130">successUserCount</span></span>|<span data-ttu-id="4c21e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="4c21e-131">Int32</span></span>|<span data-ttu-id="4c21e-132">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="4c21e-132">Success user count.</span></span>|
|<span data-ttu-id="4c21e-133">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="4c21e-133">errorUserCount</span></span>|<span data-ttu-id="4c21e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="4c21e-134">Int32</span></span>|<span data-ttu-id="4c21e-135">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="4c21e-135">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c21e-136">Relações</span><span class="sxs-lookup"><span data-stu-id="4c21e-136">Relationships</span></span>
<span data-ttu-id="4c21e-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4c21e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c21e-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c21e-138">JSON Representation</span></span>
<span data-ttu-id="4c21e-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c21e-139">Here is a JSON representation of the resource.</span></span>
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





