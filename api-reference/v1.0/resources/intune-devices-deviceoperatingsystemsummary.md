---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53c806e250d6b201e6dfe49d90685c4144913182
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250401"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="37fbb-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="37fbb-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="37fbb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37fbb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37fbb-105">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37fbb-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="37fbb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37fbb-106">Properties</span></span>
|<span data-ttu-id="37fbb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37fbb-107">Property</span></span>|<span data-ttu-id="37fbb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="37fbb-108">Type</span></span>|<span data-ttu-id="37fbb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="37fbb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37fbb-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="37fbb-110">androidCount</span></span>|<span data-ttu-id="37fbb-111">Int32</span><span class="sxs-lookup"><span data-stu-id="37fbb-111">Int32</span></span>|<span data-ttu-id="37fbb-112">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="37fbb-112">Number of android device count.</span></span>|
|<span data-ttu-id="37fbb-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="37fbb-113">iosCount</span></span>|<span data-ttu-id="37fbb-114">Int32</span><span class="sxs-lookup"><span data-stu-id="37fbb-114">Int32</span></span>|<span data-ttu-id="37fbb-115">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="37fbb-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="37fbb-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="37fbb-116">macOSCount</span></span>|<span data-ttu-id="37fbb-117">Int32</span><span class="sxs-lookup"><span data-stu-id="37fbb-117">Int32</span></span>|<span data-ttu-id="37fbb-118">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="37fbb-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="37fbb-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="37fbb-119">windowsMobileCount</span></span>|<span data-ttu-id="37fbb-120">Int32</span><span class="sxs-lookup"><span data-stu-id="37fbb-120">Int32</span></span>|<span data-ttu-id="37fbb-121">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="37fbb-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="37fbb-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="37fbb-122">windowsCount</span></span>|<span data-ttu-id="37fbb-123">Int32</span><span class="sxs-lookup"><span data-stu-id="37fbb-123">Int32</span></span>|<span data-ttu-id="37fbb-124">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="37fbb-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="37fbb-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="37fbb-125">unknownCount</span></span>|<span data-ttu-id="37fbb-126">Int32</span><span class="sxs-lookup"><span data-stu-id="37fbb-126">Int32</span></span>|<span data-ttu-id="37fbb-127">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="37fbb-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37fbb-128">Relações</span><span class="sxs-lookup"><span data-stu-id="37fbb-128">Relationships</span></span>
<span data-ttu-id="37fbb-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37fbb-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37fbb-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37fbb-130">JSON Representation</span></span>
<span data-ttu-id="37fbb-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37fbb-131">Here is a JSON representation of the resource.</span></span>
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



