---
title: tipo de recurso deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c8147bfe8033a84df4493be1ac5c5672d2249adb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081549"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="747ff-103">tipo de recurso deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="747ff-103">deviceManagementScriptRunSummary resource type</span></span>

<span data-ttu-id="747ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="747ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="747ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="747ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="747ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="747ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="747ff-107">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="747ff-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="747ff-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="747ff-108">Methods</span></span>
|<span data-ttu-id="747ff-109">Método</span><span class="sxs-lookup"><span data-stu-id="747ff-109">Method</span></span>|<span data-ttu-id="747ff-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="747ff-110">Return Type</span></span>|<span data-ttu-id="747ff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="747ff-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="747ff-112">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="747ff-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="747ff-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="747ff-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="747ff-114">Leia as propriedades e as relações do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="747ff-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="747ff-115">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="747ff-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="747ff-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="747ff-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="747ff-117">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="747ff-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="747ff-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="747ff-118">Properties</span></span>
|<span data-ttu-id="747ff-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="747ff-119">Property</span></span>|<span data-ttu-id="747ff-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="747ff-120">Type</span></span>|<span data-ttu-id="747ff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="747ff-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="747ff-122">id</span><span class="sxs-lookup"><span data-stu-id="747ff-122">id</span></span>|<span data-ttu-id="747ff-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="747ff-123">String</span></span>|<span data-ttu-id="747ff-124">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="747ff-124">Key of the device management script run summary entity.</span></span> <span data-ttu-id="747ff-125">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="747ff-125">This property is read-only.</span></span>|
|<span data-ttu-id="747ff-126">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="747ff-126">successDeviceCount</span></span>|<span data-ttu-id="747ff-127">Int32</span><span class="sxs-lookup"><span data-stu-id="747ff-127">Int32</span></span>|<span data-ttu-id="747ff-128">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="747ff-128">Success device count.</span></span>|
|<span data-ttu-id="747ff-129">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="747ff-129">errorDeviceCount</span></span>|<span data-ttu-id="747ff-130">Int32</span><span class="sxs-lookup"><span data-stu-id="747ff-130">Int32</span></span>|<span data-ttu-id="747ff-131">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="747ff-131">Error device count.</span></span>|
|<span data-ttu-id="747ff-132">successUserCount</span><span class="sxs-lookup"><span data-stu-id="747ff-132">successUserCount</span></span>|<span data-ttu-id="747ff-133">Int32</span><span class="sxs-lookup"><span data-stu-id="747ff-133">Int32</span></span>|<span data-ttu-id="747ff-134">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="747ff-134">Success user count.</span></span>|
|<span data-ttu-id="747ff-135">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="747ff-135">errorUserCount</span></span>|<span data-ttu-id="747ff-136">Int32</span><span class="sxs-lookup"><span data-stu-id="747ff-136">Int32</span></span>|<span data-ttu-id="747ff-137">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="747ff-137">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="747ff-138">Relações</span><span class="sxs-lookup"><span data-stu-id="747ff-138">Relationships</span></span>
<span data-ttu-id="747ff-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="747ff-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="747ff-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="747ff-140">JSON Representation</span></span>
<span data-ttu-id="747ff-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="747ff-141">Here is a JSON representation of the resource.</span></span>
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






