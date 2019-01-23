---
title: tipo de recurso de deviceManagementScriptRunSummary
description: Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f49e08c0f6351133b953e566ba8e89afe945e990
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423850"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="9b792-103">tipo de recurso de deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9b792-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="9b792-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9b792-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9b792-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9b792-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b792-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9b792-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b792-107">Contém propriedades para o resumo de execução de um script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b792-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="9b792-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9b792-108">Methods</span></span>
|<span data-ttu-id="9b792-109">Método</span><span class="sxs-lookup"><span data-stu-id="9b792-109">Method</span></span>|<span data-ttu-id="9b792-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9b792-110">Return Type</span></span>|<span data-ttu-id="9b792-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b792-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b792-112">Obter deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9b792-112">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[<span data-ttu-id="9b792-113">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9b792-113">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="9b792-114">Leia as propriedades e os relacionamentos do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9b792-114">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="9b792-115">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9b792-115">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[<span data-ttu-id="9b792-116">deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="9b792-116">deviceManagementScriptRunSummary</span></span>](../resources/intune-devices-devicemanagementscriptrunsummary.md)|<span data-ttu-id="9b792-117">Atualize as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9b792-117">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b792-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b792-118">Properties</span></span>
|<span data-ttu-id="9b792-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b792-119">Property</span></span>|<span data-ttu-id="9b792-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b792-120">Type</span></span>|<span data-ttu-id="9b792-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b792-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b792-122">id</span><span class="sxs-lookup"><span data-stu-id="9b792-122">id</span></span>|<span data-ttu-id="9b792-123">String</span><span class="sxs-lookup"><span data-stu-id="9b792-123">String</span></span>|<span data-ttu-id="9b792-124">Chave do script de gerenciamento de dispositivo execute entidade resumida.</span><span class="sxs-lookup"><span data-stu-id="9b792-124">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="9b792-125">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9b792-125">successDeviceCount</span></span>|<span data-ttu-id="9b792-126">Int32</span><span class="sxs-lookup"><span data-stu-id="9b792-126">Int32</span></span>|<span data-ttu-id="9b792-127">Contagem de sucesso do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b792-127">Success device count.</span></span>|
|<span data-ttu-id="9b792-128">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9b792-128">errorDeviceCount</span></span>|<span data-ttu-id="9b792-129">Int32</span><span class="sxs-lookup"><span data-stu-id="9b792-129">Int32</span></span>|<span data-ttu-id="9b792-130">Contagem de erros de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9b792-130">Error device count.</span></span>|
|<span data-ttu-id="9b792-131">successUserCount</span><span class="sxs-lookup"><span data-stu-id="9b792-131">successUserCount</span></span>|<span data-ttu-id="9b792-132">Int32</span><span class="sxs-lookup"><span data-stu-id="9b792-132">Int32</span></span>|<span data-ttu-id="9b792-133">Contagem de usuário de sucesso.</span><span class="sxs-lookup"><span data-stu-id="9b792-133">Success user count.</span></span>|
|<span data-ttu-id="9b792-134">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="9b792-134">errorUserCount</span></span>|<span data-ttu-id="9b792-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9b792-135">Int32</span></span>|<span data-ttu-id="9b792-136">Contagem de erros de usuário.</span><span class="sxs-lookup"><span data-stu-id="9b792-136">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b792-137">Relações</span><span class="sxs-lookup"><span data-stu-id="9b792-137">Relationships</span></span>
<span data-ttu-id="9b792-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b792-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b792-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b792-139">JSON Representation</span></span>
<span data-ttu-id="9b792-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b792-140">Here is a JSON representation of the resource.</span></span>
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




