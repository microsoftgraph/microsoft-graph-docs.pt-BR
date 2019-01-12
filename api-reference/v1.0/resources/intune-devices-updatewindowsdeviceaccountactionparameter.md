---
title: Tipo de recurso updateWindowsDeviceAccountActionParameter
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f62dce1364fca28e85b728e0b7571906488ebbee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986674"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="a8956-103">Tipo de recurso updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="a8956-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="a8956-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8956-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8956-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8956-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a8956-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8956-106">Properties</span></span>
|<span data-ttu-id="a8956-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8956-107">Property</span></span>|<span data-ttu-id="a8956-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8956-108">Type</span></span>|<span data-ttu-id="a8956-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8956-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8956-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="a8956-110">deviceAccount</span></span>|[<span data-ttu-id="a8956-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="a8956-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="a8956-112">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8956-112">Not yet documented</span></span>|
|<span data-ttu-id="a8956-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="a8956-113">passwordRotationEnabled</span></span>|<span data-ttu-id="a8956-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="a8956-114">Boolean</span></span>|<span data-ttu-id="a8956-115">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8956-115">Not yet documented</span></span>|
|<span data-ttu-id="a8956-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="a8956-116">calendarSyncEnabled</span></span>|<span data-ttu-id="a8956-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="a8956-117">Boolean</span></span>|<span data-ttu-id="a8956-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8956-118">Not yet documented</span></span>|
|<span data-ttu-id="a8956-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="a8956-119">deviceAccountEmail</span></span>|<span data-ttu-id="a8956-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8956-120">String</span></span>|<span data-ttu-id="a8956-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8956-121">Not yet documented</span></span>|
|<span data-ttu-id="a8956-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="a8956-122">exchangeServer</span></span>|<span data-ttu-id="a8956-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8956-123">String</span></span>|<span data-ttu-id="a8956-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8956-124">Not yet documented</span></span>|
|<span data-ttu-id="a8956-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="a8956-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="a8956-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8956-126">String</span></span>|<span data-ttu-id="a8956-127">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a8956-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8956-128">Relações</span><span class="sxs-lookup"><span data-stu-id="a8956-128">Relationships</span></span>
<span data-ttu-id="a8956-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8956-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8956-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8956-130">JSON Representation</span></span>
<span data-ttu-id="a8956-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8956-131">Here is a JSON representation of the resource.</span></span>
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



