---
title: Tipo de recurso activateDeviceEsimActionResult
description: Ativar o resultado da ação do eSIM do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c0a391ee52a84b49e105e90eff57510b8ae1010
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666879"
---
# <a name="activatedeviceesimactionresult-resource-type"></a><span data-ttu-id="2fa5a-103">Tipo de recurso activateDeviceEsimActionResult</span><span class="sxs-lookup"><span data-stu-id="2fa5a-103">activateDeviceEsimActionResult resource type</span></span>

<span data-ttu-id="2fa5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fa5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fa5a-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2fa5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fa5a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fa5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fa5a-107">Ativar o resultado da ação do eSIM do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2fa5a-107">Activate device eSIM action result</span></span>


<span data-ttu-id="2fa5a-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2fa5a-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2fa5a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fa5a-109">Properties</span></span>
|<span data-ttu-id="2fa5a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fa5a-110">Property</span></span>|<span data-ttu-id="2fa5a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fa5a-111">Type</span></span>|<span data-ttu-id="2fa5a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fa5a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fa5a-113">actionName</span><span class="sxs-lookup"><span data-stu-id="2fa5a-113">actionName</span></span>|<span data-ttu-id="2fa5a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fa5a-114">String</span></span>|<span data-ttu-id="2fa5a-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2fa5a-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2fa5a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2fa5a-116">actionState</span></span>|[<span data-ttu-id="2fa5a-117">actionState</span><span class="sxs-lookup"><span data-stu-id="2fa5a-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2fa5a-118">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2fa5a-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2fa5a-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="2fa5a-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2fa5a-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa5a-120">startDateTime</span></span>|<span data-ttu-id="2fa5a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa5a-121">DateTimeOffset</span></span>|<span data-ttu-id="2fa5a-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2fa5a-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2fa5a-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa5a-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="2fa5a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa5a-124">DateTimeOffset</span></span>|<span data-ttu-id="2fa5a-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2fa5a-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2fa5a-126">carrierUrl</span><span class="sxs-lookup"><span data-stu-id="2fa5a-126">carrierUrl</span></span>|<span data-ttu-id="2fa5a-127">String</span><span class="sxs-lookup"><span data-stu-id="2fa5a-127">String</span></span>|<span data-ttu-id="2fa5a-128">Url da operadora para ativar o eSIM do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2fa5a-128">Carrier Url to activate the device eSIM</span></span> |

## <a name="relationships"></a><span data-ttu-id="2fa5a-129">Relações</span><span class="sxs-lookup"><span data-stu-id="2fa5a-129">Relationships</span></span>
<span data-ttu-id="2fa5a-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2fa5a-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fa5a-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fa5a-131">JSON Representation</span></span>
<span data-ttu-id="2fa5a-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fa5a-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.activateDeviceEsimActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activateDeviceEsimActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "carrierUrl": "String"
}
```




