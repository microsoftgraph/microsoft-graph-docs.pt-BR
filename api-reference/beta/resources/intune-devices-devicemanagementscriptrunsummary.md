---
title: tipo de recurso deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce974f3d5e024a9559f454e8837fd04183e4de9d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784892"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="c723a-103">tipo de recurso deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c723a-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="c723a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c723a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c723a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c723a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c723a-106">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c723a-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="c723a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c723a-107">Methods</span></span>
|<span data-ttu-id="c723a-108">Método</span><span class="sxs-lookup"><span data-stu-id="c723a-108">Method</span></span>|<span data-ttu-id="c723a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c723a-109">Return Type</span></span>|<span data-ttu-id="c723a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c723a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c723a-111">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c723a-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="c723a-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c723a-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="c723a-113">Leia as propriedades e as relações do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c723a-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="c723a-114">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c723a-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="c723a-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c723a-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="c723a-116">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c723a-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c723a-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c723a-117">Properties</span></span>
|<span data-ttu-id="c723a-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c723a-118">Property</span></span>|<span data-ttu-id="c723a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c723a-119">Type</span></span>|<span data-ttu-id="c723a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c723a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c723a-121">id</span><span class="sxs-lookup"><span data-stu-id="c723a-121">id</span></span>|<span data-ttu-id="c723a-122">String</span><span class="sxs-lookup"><span data-stu-id="c723a-122">String</span></span>|<span data-ttu-id="c723a-123">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c723a-123">Key of the device management script run summary entity.</span></span> <span data-ttu-id="c723a-124">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c723a-124">This property is read-only.</span></span>|
|<span data-ttu-id="c723a-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c723a-125">successDeviceCount</span></span>|<span data-ttu-id="c723a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="c723a-126">Int32</span></span>|<span data-ttu-id="c723a-127">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="c723a-127">Success device count.</span></span>|
|<span data-ttu-id="c723a-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c723a-128">errorDeviceCount</span></span>|<span data-ttu-id="c723a-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c723a-129">Int32</span></span>|<span data-ttu-id="c723a-130">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="c723a-130">Error device count.</span></span>|
|<span data-ttu-id="c723a-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="c723a-131">successUserCount</span></span>|<span data-ttu-id="c723a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="c723a-132">Int32</span></span>|<span data-ttu-id="c723a-133">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="c723a-133">Success user count.</span></span>|
|<span data-ttu-id="c723a-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="c723a-134">errorUserCount</span></span>|<span data-ttu-id="c723a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="c723a-135">Int32</span></span>|<span data-ttu-id="c723a-136">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="c723a-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c723a-137">Relações</span><span class="sxs-lookup"><span data-stu-id="c723a-137">Relationships</span></span>
<span data-ttu-id="c723a-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c723a-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c723a-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c723a-139">JSON Representation</span></span>
<span data-ttu-id="c723a-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c723a-140">Here is a JSON representation of the resource.</span></span>
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



