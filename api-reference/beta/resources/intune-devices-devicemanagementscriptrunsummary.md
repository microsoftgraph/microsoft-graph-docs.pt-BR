---
title: tipo de recurso deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199b9efcdc3ea862502ea22d845480d990c99caf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995305"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="cf27e-103">tipo de recurso deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="cf27e-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="cf27e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf27e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf27e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf27e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf27e-106">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cf27e-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="cf27e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cf27e-107">Methods</span></span>
|<span data-ttu-id="cf27e-108">Método</span><span class="sxs-lookup"><span data-stu-id="cf27e-108">Method</span></span>|<span data-ttu-id="cf27e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cf27e-109">Return Type</span></span>|<span data-ttu-id="cf27e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf27e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf27e-111">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="cf27e-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="cf27e-112">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="cf27e-112">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="cf27e-113">Leia as propriedades e as relações do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cf27e-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="cf27e-114">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="cf27e-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="cf27e-115">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="cf27e-115">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="cf27e-116">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cf27e-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf27e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf27e-117">Properties</span></span>
|<span data-ttu-id="cf27e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf27e-118">Property</span></span>|<span data-ttu-id="cf27e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf27e-119">Type</span></span>|<span data-ttu-id="cf27e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf27e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf27e-121">id</span><span class="sxs-lookup"><span data-stu-id="cf27e-121">id</span></span>|<span data-ttu-id="cf27e-122">String</span><span class="sxs-lookup"><span data-stu-id="cf27e-122">String</span></span>|<span data-ttu-id="cf27e-123">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cf27e-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="cf27e-124">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf27e-124">successDeviceCount</span></span>|<span data-ttu-id="cf27e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cf27e-125">Int32</span></span>|<span data-ttu-id="cf27e-126">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="cf27e-126">Success device count.</span></span>|
|<span data-ttu-id="cf27e-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf27e-127">errorDeviceCount</span></span>|<span data-ttu-id="cf27e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="cf27e-128">Int32</span></span>|<span data-ttu-id="cf27e-129">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="cf27e-129">Error device count.</span></span>|
|<span data-ttu-id="cf27e-130">successUserCount</span><span class="sxs-lookup"><span data-stu-id="cf27e-130">successUserCount</span></span>|<span data-ttu-id="cf27e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="cf27e-131">Int32</span></span>|<span data-ttu-id="cf27e-132">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="cf27e-132">Success user count.</span></span>|
|<span data-ttu-id="cf27e-133">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="cf27e-133">errorUserCount</span></span>|<span data-ttu-id="cf27e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="cf27e-134">Int32</span></span>|<span data-ttu-id="cf27e-135">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="cf27e-135">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf27e-136">Relações</span><span class="sxs-lookup"><span data-stu-id="cf27e-136">Relationships</span></span>
<span data-ttu-id="cf27e-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf27e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf27e-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf27e-138">JSON Representation</span></span>
<span data-ttu-id="cf27e-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf27e-139">Here is a JSON representation of the resource.</span></span>
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





