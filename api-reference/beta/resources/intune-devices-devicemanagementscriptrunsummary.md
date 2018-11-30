---
title: tipo de recurso de deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
ms.openlocfilehash: 9269ae5f3f6fc889cb02ad90e2897c9a3e979241
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038943"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="15b5f-103">tipo de recurso de deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="15b5f-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="15b5f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="15b5f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15b5f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15b5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15b5f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="15b5f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15b5f-107">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15b5f-107">Contains properties for the run summary of a device management script.</span></span>
## <a name="methods"></a><span data-ttu-id="15b5f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="15b5f-108">Methods</span></span>
|<span data-ttu-id="15b5f-109">Método</span><span class="sxs-lookup"><span data-stu-id="15b5f-109">Method</span></span>|<span data-ttu-id="15b5f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="15b5f-110">Return Type</span></span>|<span data-ttu-id="15b5f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="15b5f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15b5f-112">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="15b5f-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="15b5f-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="15b5f-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="15b5f-114">Leia as propriedades e os relacionamentos do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="15b5f-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="15b5f-115">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="15b5f-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="15b5f-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="15b5f-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="15b5f-117">Atualize as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="15b5f-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="15b5f-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15b5f-118">Properties</span></span>
|<span data-ttu-id="15b5f-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15b5f-119">Property</span></span>|<span data-ttu-id="15b5f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="15b5f-120">Type</span></span>|<span data-ttu-id="15b5f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="15b5f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15b5f-122">id</span><span class="sxs-lookup"><span data-stu-id="15b5f-122">id</span></span>|<span data-ttu-id="15b5f-123">String</span><span class="sxs-lookup"><span data-stu-id="15b5f-123">String</span></span>|<span data-ttu-id="15b5f-124">Chave do script de gerenciamento de dispositivo execute entidade resumida.</span><span class="sxs-lookup"><span data-stu-id="15b5f-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="15b5f-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15b5f-125">successDeviceCount</span></span>|<span data-ttu-id="15b5f-126">Int32</span><span class="sxs-lookup"><span data-stu-id="15b5f-126">Int32</span></span>|<span data-ttu-id="15b5f-127">Contagem de sucesso do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15b5f-127">Success device count.</span></span>|
|<span data-ttu-id="15b5f-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="15b5f-128">errorDeviceCount</span></span>|<span data-ttu-id="15b5f-129">Int32</span><span class="sxs-lookup"><span data-stu-id="15b5f-129">Int32</span></span>|<span data-ttu-id="15b5f-130">Contagem de erros de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15b5f-130">Error device count.</span></span>|
|<span data-ttu-id="15b5f-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="15b5f-131">successUserCount</span></span>|<span data-ttu-id="15b5f-132">Int32</span><span class="sxs-lookup"><span data-stu-id="15b5f-132">Int32</span></span>|<span data-ttu-id="15b5f-133">Contagem de usuário de sucesso.</span><span class="sxs-lookup"><span data-stu-id="15b5f-133">Success user count.</span></span>|
|<span data-ttu-id="15b5f-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="15b5f-134">errorUserCount</span></span>|<span data-ttu-id="15b5f-135">Int32</span><span class="sxs-lookup"><span data-stu-id="15b5f-135">Int32</span></span>|<span data-ttu-id="15b5f-136">Contagem de erros de usuário.</span><span class="sxs-lookup"><span data-stu-id="15b5f-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15b5f-137">Relações</span><span class="sxs-lookup"><span data-stu-id="15b5f-137">Relationships</span></span>
<span data-ttu-id="15b5f-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15b5f-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15b5f-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15b5f-139">JSON Representation</span></span>
<span data-ttu-id="15b5f-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15b5f-140">Here is a JSON representation of the resource.</span></span>
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





