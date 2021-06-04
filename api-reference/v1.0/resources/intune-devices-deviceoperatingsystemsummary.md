---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9dfce6c0947fffd861ae1cda205c1011a7500471
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754564"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="3e547-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="3e547-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="3e547-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e547-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e547-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e547-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e547-106">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e547-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="3e547-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e547-107">Properties</span></span>
|<span data-ttu-id="3e547-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e547-108">Property</span></span>|<span data-ttu-id="3e547-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e547-109">Type</span></span>|<span data-ttu-id="3e547-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e547-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e547-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="3e547-111">androidCount</span></span>|<span data-ttu-id="3e547-112">Int32</span><span class="sxs-lookup"><span data-stu-id="3e547-112">Int32</span></span>|<span data-ttu-id="3e547-113">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="3e547-113">Number of android device count.</span></span>|
|<span data-ttu-id="3e547-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="3e547-114">iosCount</span></span>|<span data-ttu-id="3e547-115">Int32</span><span class="sxs-lookup"><span data-stu-id="3e547-115">Int32</span></span>|<span data-ttu-id="3e547-116">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="3e547-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="3e547-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="3e547-117">macOSCount</span></span>|<span data-ttu-id="3e547-118">Int32</span><span class="sxs-lookup"><span data-stu-id="3e547-118">Int32</span></span>|<span data-ttu-id="3e547-119">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="3e547-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="3e547-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="3e547-120">windowsMobileCount</span></span>|<span data-ttu-id="3e547-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3e547-121">Int32</span></span>|<span data-ttu-id="3e547-122">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="3e547-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="3e547-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="3e547-123">windowsCount</span></span>|<span data-ttu-id="3e547-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3e547-124">Int32</span></span>|<span data-ttu-id="3e547-125">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="3e547-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="3e547-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="3e547-126">unknownCount</span></span>|<span data-ttu-id="3e547-127">Int32</span><span class="sxs-lookup"><span data-stu-id="3e547-127">Int32</span></span>|<span data-ttu-id="3e547-128">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="3e547-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e547-129">Relações</span><span class="sxs-lookup"><span data-stu-id="3e547-129">Relationships</span></span>
<span data-ttu-id="3e547-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3e547-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e547-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e547-131">JSON Representation</span></span>
<span data-ttu-id="3e547-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e547-132">Here is a JSON representation of the resource.</span></span>
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




