---
title: Tipo de recurso updateWindowsDeviceAccountActionParameter
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95ed870849faebec289cd59ba9d58eee67d27fd9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526283"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="162fb-103">Tipo de recurso updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="162fb-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="162fb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="162fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="162fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="162fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="162fb-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="162fb-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="162fb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="162fb-107">Properties</span></span>
|<span data-ttu-id="162fb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="162fb-108">Property</span></span>|<span data-ttu-id="162fb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="162fb-109">Type</span></span>|<span data-ttu-id="162fb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="162fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="162fb-111">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="162fb-111">deviceAccount</span></span>|[<span data-ttu-id="162fb-112">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="162fb-112">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="162fb-113">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="162fb-113">Not yet documented</span></span>|
|<span data-ttu-id="162fb-114">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="162fb-114">passwordRotationEnabled</span></span>|<span data-ttu-id="162fb-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="162fb-115">Boolean</span></span>|<span data-ttu-id="162fb-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="162fb-116">Not yet documented</span></span>|
|<span data-ttu-id="162fb-117">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="162fb-117">calendarSyncEnabled</span></span>|<span data-ttu-id="162fb-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="162fb-118">Boolean</span></span>|<span data-ttu-id="162fb-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="162fb-119">Not yet documented</span></span>|
|<span data-ttu-id="162fb-120">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="162fb-120">deviceAccountEmail</span></span>|<span data-ttu-id="162fb-121">String</span><span class="sxs-lookup"><span data-stu-id="162fb-121">String</span></span>|<span data-ttu-id="162fb-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="162fb-122">Not yet documented</span></span>|
|<span data-ttu-id="162fb-123">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="162fb-123">exchangeServer</span></span>|<span data-ttu-id="162fb-124">String</span><span class="sxs-lookup"><span data-stu-id="162fb-124">String</span></span>|<span data-ttu-id="162fb-125">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="162fb-125">Not yet documented</span></span>|
|<span data-ttu-id="162fb-126">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="162fb-126">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="162fb-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="162fb-127">String</span></span>|<span data-ttu-id="162fb-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="162fb-128">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="162fb-129">Relações</span><span class="sxs-lookup"><span data-stu-id="162fb-129">Relationships</span></span>
<span data-ttu-id="162fb-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="162fb-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="162fb-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="162fb-131">JSON Representation</span></span>
<span data-ttu-id="162fb-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="162fb-132">Here is a JSON representation of the resource.</span></span>
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





