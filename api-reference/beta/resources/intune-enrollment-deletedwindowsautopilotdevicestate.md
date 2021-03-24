---
title: Tipo de recurso deletedWindowsAutopilotDeviceState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87113449f0c00722f3aa1d3a1e614873524d43a6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146739"
---
# <a name="deletedwindowsautopilotdevicestate-resource-type"></a><span data-ttu-id="c1859-103">Tipo de recurso deletedWindowsAutopilotDeviceState</span><span class="sxs-lookup"><span data-stu-id="c1859-103">deletedWindowsAutopilotDeviceState resource type</span></span>

<span data-ttu-id="c1859-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1859-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1859-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1859-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1859-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1859-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1859-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c1859-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c1859-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1859-108">Properties</span></span>
|<span data-ttu-id="c1859-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1859-109">Property</span></span>|<span data-ttu-id="c1859-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1859-110">Type</span></span>|<span data-ttu-id="c1859-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1859-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1859-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="c1859-112">serialNumber</span></span>|<span data-ttu-id="c1859-113">String</span><span class="sxs-lookup"><span data-stu-id="c1859-113">String</span></span>|<span data-ttu-id="c1859-114">Número de série do dispositivo Autopilot</span><span class="sxs-lookup"><span data-stu-id="c1859-114">Autopilot Device Serial Number</span></span>|
|<span data-ttu-id="c1859-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="c1859-115">deviceRegistrationId</span></span>|<span data-ttu-id="c1859-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1859-116">String</span></span>|<span data-ttu-id="c1859-117">ID de Registro de Dispositivo ZTD .</span><span class="sxs-lookup"><span data-stu-id="c1859-117">ZTD Device Registration ID .</span></span>|
|<span data-ttu-id="c1859-118">deletionState</span><span class="sxs-lookup"><span data-stu-id="c1859-118">deletionState</span></span>|[<span data-ttu-id="c1859-119">windowsAutopilotDeviceDeletionState</span><span class="sxs-lookup"><span data-stu-id="c1859-119">windowsAutopilotDeviceDeletionState</span></span>](../resources/intune-enrollment-windowsautopilotdevicedeletionstate.md)|<span data-ttu-id="c1859-120">Estado de exclusão de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1859-120">Device deletion state.</span></span> <span data-ttu-id="c1859-121">Os valores possíveis são: `unknown`, `failed`, `accepted`, `error`.</span><span class="sxs-lookup"><span data-stu-id="c1859-121">Possible values are: `unknown`, `failed`, `accepted`, `error`.</span></span>|
|<span data-ttu-id="c1859-122">errorMessage</span><span class="sxs-lookup"><span data-stu-id="c1859-122">errorMessage</span></span>|<span data-ttu-id="c1859-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1859-123">String</span></span>|<span data-ttu-id="c1859-124">Mensagem de erro de exclusão de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1859-124">Device deletion error message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1859-125">Relações</span><span class="sxs-lookup"><span data-stu-id="c1859-125">Relationships</span></span>
<span data-ttu-id="c1859-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1859-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1859-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1859-127">JSON Representation</span></span>
<span data-ttu-id="c1859-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1859-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deletedWindowsAutopilotDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deletedWindowsAutopilotDeviceState",
  "serialNumber": "String",
  "deviceRegistrationId": "String",
  "deletionState": "String",
  "errorMessage": "String"
}
```




