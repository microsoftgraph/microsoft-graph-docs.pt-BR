---
title: Tipo de recurso updateWindowsDeviceAccountActionParameter
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 33b4b9e62b1038eb3b9e97b01a3d7b38906b605c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356888"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="8643e-103">Tipo de recurso updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="8643e-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="8643e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8643e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8643e-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8643e-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8643e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8643e-106">Properties</span></span>
|<span data-ttu-id="8643e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8643e-107">Property</span></span>|<span data-ttu-id="8643e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8643e-108">Type</span></span>|<span data-ttu-id="8643e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8643e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8643e-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="8643e-110">deviceAccount</span></span>|[<span data-ttu-id="8643e-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="8643e-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="8643e-112">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8643e-112">Not yet documented</span></span>|
|<span data-ttu-id="8643e-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="8643e-113">passwordRotationEnabled</span></span>|<span data-ttu-id="8643e-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="8643e-114">Boolean</span></span>|<span data-ttu-id="8643e-115">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8643e-115">Not yet documented</span></span>|
|<span data-ttu-id="8643e-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="8643e-116">calendarSyncEnabled</span></span>|<span data-ttu-id="8643e-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="8643e-117">Boolean</span></span>|<span data-ttu-id="8643e-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8643e-118">Not yet documented</span></span>|
|<span data-ttu-id="8643e-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="8643e-119">deviceAccountEmail</span></span>|<span data-ttu-id="8643e-120">String</span><span class="sxs-lookup"><span data-stu-id="8643e-120">String</span></span>|<span data-ttu-id="8643e-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8643e-121">Not yet documented</span></span>|
|<span data-ttu-id="8643e-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="8643e-122">exchangeServer</span></span>|<span data-ttu-id="8643e-123">String</span><span class="sxs-lookup"><span data-stu-id="8643e-123">String</span></span>|<span data-ttu-id="8643e-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8643e-124">Not yet documented</span></span>|
|<span data-ttu-id="8643e-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="8643e-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="8643e-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8643e-126">String</span></span>|<span data-ttu-id="8643e-127">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8643e-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="8643e-128">Relações</span><span class="sxs-lookup"><span data-stu-id="8643e-128">Relationships</span></span>
<span data-ttu-id="8643e-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8643e-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8643e-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8643e-130">JSON Representation</span></span>
<span data-ttu-id="8643e-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8643e-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```




