---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8e61898cb7dfd8f2f058beaf668763ecda27928
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968397"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="6ca04-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="6ca04-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="6ca04-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ca04-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ca04-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ca04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ca04-106">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ca04-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="6ca04-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ca04-107">Properties</span></span>
|<span data-ttu-id="6ca04-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ca04-108">Property</span></span>|<span data-ttu-id="6ca04-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ca04-109">Type</span></span>|<span data-ttu-id="6ca04-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ca04-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ca04-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="6ca04-111">androidCount</span></span>|<span data-ttu-id="6ca04-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6ca04-112">Int32</span></span>|<span data-ttu-id="6ca04-113">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="6ca04-113">Number of android device count.</span></span>|
|<span data-ttu-id="6ca04-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="6ca04-114">iosCount</span></span>|<span data-ttu-id="6ca04-115">Int32</span><span class="sxs-lookup"><span data-stu-id="6ca04-115">Int32</span></span>|<span data-ttu-id="6ca04-116">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="6ca04-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="6ca04-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="6ca04-117">macOSCount</span></span>|<span data-ttu-id="6ca04-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6ca04-118">Int32</span></span>|<span data-ttu-id="6ca04-119">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="6ca04-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="6ca04-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="6ca04-120">windowsMobileCount</span></span>|<span data-ttu-id="6ca04-121">Int32</span><span class="sxs-lookup"><span data-stu-id="6ca04-121">Int32</span></span>|<span data-ttu-id="6ca04-122">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="6ca04-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="6ca04-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="6ca04-123">windowsCount</span></span>|<span data-ttu-id="6ca04-124">Int32</span><span class="sxs-lookup"><span data-stu-id="6ca04-124">Int32</span></span>|<span data-ttu-id="6ca04-125">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="6ca04-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="6ca04-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="6ca04-126">unknownCount</span></span>|<span data-ttu-id="6ca04-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6ca04-127">Int32</span></span>|<span data-ttu-id="6ca04-128">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="6ca04-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ca04-129">Relações</span><span class="sxs-lookup"><span data-stu-id="6ca04-129">Relationships</span></span>
<span data-ttu-id="6ca04-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ca04-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ca04-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ca04-131">JSON Representation</span></span>
<span data-ttu-id="6ca04-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ca04-132">Here is a JSON representation of the resource.</span></span>
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





