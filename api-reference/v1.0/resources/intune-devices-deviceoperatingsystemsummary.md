---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2147034c060fa15e8e799d5ddbe72aabe635af08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975640"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="179f6-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="179f6-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="179f6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="179f6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="179f6-105">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="179f6-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="179f6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="179f6-106">Properties</span></span>
|<span data-ttu-id="179f6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="179f6-107">Property</span></span>|<span data-ttu-id="179f6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="179f6-108">Type</span></span>|<span data-ttu-id="179f6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="179f6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="179f6-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="179f6-110">androidCount</span></span>|<span data-ttu-id="179f6-111">Int32</span><span class="sxs-lookup"><span data-stu-id="179f6-111">Int32</span></span>|<span data-ttu-id="179f6-112">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="179f6-112">Number of android device count.</span></span>|
|<span data-ttu-id="179f6-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="179f6-113">iosCount</span></span>|<span data-ttu-id="179f6-114">Int32</span><span class="sxs-lookup"><span data-stu-id="179f6-114">Int32</span></span>|<span data-ttu-id="179f6-115">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="179f6-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="179f6-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="179f6-116">macOSCount</span></span>|<span data-ttu-id="179f6-117">Int32</span><span class="sxs-lookup"><span data-stu-id="179f6-117">Int32</span></span>|<span data-ttu-id="179f6-118">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="179f6-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="179f6-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="179f6-119">windowsMobileCount</span></span>|<span data-ttu-id="179f6-120">Int32</span><span class="sxs-lookup"><span data-stu-id="179f6-120">Int32</span></span>|<span data-ttu-id="179f6-121">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="179f6-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="179f6-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="179f6-122">windowsCount</span></span>|<span data-ttu-id="179f6-123">Int32</span><span class="sxs-lookup"><span data-stu-id="179f6-123">Int32</span></span>|<span data-ttu-id="179f6-124">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="179f6-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="179f6-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="179f6-125">unknownCount</span></span>|<span data-ttu-id="179f6-126">Int32</span><span class="sxs-lookup"><span data-stu-id="179f6-126">Int32</span></span>|<span data-ttu-id="179f6-127">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="179f6-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="179f6-128">Relações</span><span class="sxs-lookup"><span data-stu-id="179f6-128">Relationships</span></span>
<span data-ttu-id="179f6-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="179f6-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="179f6-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="179f6-130">JSON Representation</span></span>
<span data-ttu-id="179f6-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="179f6-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



