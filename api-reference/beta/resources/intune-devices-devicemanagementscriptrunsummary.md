---
title: tipo de recurso deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1780dbfd6d53cf25fdd18b3c78f0c84c39b5455d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538788"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="01f73-103">tipo de recurso deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="01f73-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="01f73-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01f73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01f73-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01f73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01f73-106">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01f73-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="01f73-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="01f73-107">Methods</span></span>
|<span data-ttu-id="01f73-108">Método</span><span class="sxs-lookup"><span data-stu-id="01f73-108">Method</span></span>|<span data-ttu-id="01f73-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="01f73-109">Return Type</span></span>|<span data-ttu-id="01f73-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="01f73-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="01f73-111">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="01f73-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="01f73-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="01f73-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="01f73-113">Leia as propriedades e as relações do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="01f73-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="01f73-114">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="01f73-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="01f73-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="01f73-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="01f73-116">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="01f73-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="01f73-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01f73-117">Properties</span></span>
|<span data-ttu-id="01f73-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01f73-118">Property</span></span>|<span data-ttu-id="01f73-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="01f73-119">Type</span></span>|<span data-ttu-id="01f73-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="01f73-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01f73-121">id</span><span class="sxs-lookup"><span data-stu-id="01f73-121">id</span></span>|<span data-ttu-id="01f73-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="01f73-122">String</span></span>|<span data-ttu-id="01f73-123">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01f73-123">Key of the device management script run summary entity.</span></span> <span data-ttu-id="01f73-124">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01f73-124">This property is read-only.</span></span>|
|<span data-ttu-id="01f73-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01f73-125">successDeviceCount</span></span>|<span data-ttu-id="01f73-126">Int32</span><span class="sxs-lookup"><span data-stu-id="01f73-126">Int32</span></span>|<span data-ttu-id="01f73-127">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="01f73-127">Success device count.</span></span>|
|<span data-ttu-id="01f73-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01f73-128">errorDeviceCount</span></span>|<span data-ttu-id="01f73-129">Int32</span><span class="sxs-lookup"><span data-stu-id="01f73-129">Int32</span></span>|<span data-ttu-id="01f73-130">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="01f73-130">Error device count.</span></span>|
|<span data-ttu-id="01f73-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="01f73-131">successUserCount</span></span>|<span data-ttu-id="01f73-132">Int32</span><span class="sxs-lookup"><span data-stu-id="01f73-132">Int32</span></span>|<span data-ttu-id="01f73-133">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="01f73-133">Success user count.</span></span>|
|<span data-ttu-id="01f73-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="01f73-134">errorUserCount</span></span>|<span data-ttu-id="01f73-135">Int32</span><span class="sxs-lookup"><span data-stu-id="01f73-135">Int32</span></span>|<span data-ttu-id="01f73-136">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="01f73-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01f73-137">Relações</span><span class="sxs-lookup"><span data-stu-id="01f73-137">Relationships</span></span>
<span data-ttu-id="01f73-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01f73-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01f73-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01f73-139">JSON Representation</span></span>
<span data-ttu-id="01f73-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01f73-140">Here is a JSON representation of the resource.</span></span>
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



