---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62fe2496e505ac0d281381b9d53604aa98094f3c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356931"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="320af-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="320af-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="320af-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="320af-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="320af-105">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="320af-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="320af-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="320af-106">Properties</span></span>
|<span data-ttu-id="320af-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="320af-107">Property</span></span>|<span data-ttu-id="320af-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="320af-108">Type</span></span>|<span data-ttu-id="320af-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="320af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="320af-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="320af-110">androidCount</span></span>|<span data-ttu-id="320af-111">Int32</span><span class="sxs-lookup"><span data-stu-id="320af-111">Int32</span></span>|<span data-ttu-id="320af-112">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="320af-112">Number of android device count.</span></span>|
|<span data-ttu-id="320af-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="320af-113">iosCount</span></span>|<span data-ttu-id="320af-114">Int32</span><span class="sxs-lookup"><span data-stu-id="320af-114">Int32</span></span>|<span data-ttu-id="320af-115">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="320af-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="320af-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="320af-116">macOSCount</span></span>|<span data-ttu-id="320af-117">Int32</span><span class="sxs-lookup"><span data-stu-id="320af-117">Int32</span></span>|<span data-ttu-id="320af-118">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="320af-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="320af-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="320af-119">windowsMobileCount</span></span>|<span data-ttu-id="320af-120">Int32</span><span class="sxs-lookup"><span data-stu-id="320af-120">Int32</span></span>|<span data-ttu-id="320af-121">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="320af-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="320af-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="320af-122">windowsCount</span></span>|<span data-ttu-id="320af-123">Int32</span><span class="sxs-lookup"><span data-stu-id="320af-123">Int32</span></span>|<span data-ttu-id="320af-124">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="320af-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="320af-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="320af-125">unknownCount</span></span>|<span data-ttu-id="320af-126">Int32</span><span class="sxs-lookup"><span data-stu-id="320af-126">Int32</span></span>|<span data-ttu-id="320af-127">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="320af-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="320af-128">Relações</span><span class="sxs-lookup"><span data-stu-id="320af-128">Relationships</span></span>
<span data-ttu-id="320af-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="320af-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="320af-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="320af-130">JSON Representation</span></span>
<span data-ttu-id="320af-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="320af-131">Here is a JSON representation of the resource.</span></span>
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




