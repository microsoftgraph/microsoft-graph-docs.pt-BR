---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 460edb4724dcff002e207d7c5df6095cc3a8f130
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453973"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="98995-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="98995-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="98995-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98995-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98995-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98995-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98995-106">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98995-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="98995-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98995-107">Properties</span></span>
|<span data-ttu-id="98995-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98995-108">Property</span></span>|<span data-ttu-id="98995-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="98995-109">Type</span></span>|<span data-ttu-id="98995-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="98995-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98995-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="98995-111">androidCount</span></span>|<span data-ttu-id="98995-112">Int32</span><span class="sxs-lookup"><span data-stu-id="98995-112">Int32</span></span>|<span data-ttu-id="98995-113">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="98995-113">Number of android device count.</span></span>|
|<span data-ttu-id="98995-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="98995-114">iosCount</span></span>|<span data-ttu-id="98995-115">Int32</span><span class="sxs-lookup"><span data-stu-id="98995-115">Int32</span></span>|<span data-ttu-id="98995-116">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="98995-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="98995-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="98995-117">macOSCount</span></span>|<span data-ttu-id="98995-118">Int32</span><span class="sxs-lookup"><span data-stu-id="98995-118">Int32</span></span>|<span data-ttu-id="98995-119">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="98995-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="98995-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="98995-120">windowsMobileCount</span></span>|<span data-ttu-id="98995-121">Int32</span><span class="sxs-lookup"><span data-stu-id="98995-121">Int32</span></span>|<span data-ttu-id="98995-122">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="98995-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="98995-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="98995-123">windowsCount</span></span>|<span data-ttu-id="98995-124">Int32</span><span class="sxs-lookup"><span data-stu-id="98995-124">Int32</span></span>|<span data-ttu-id="98995-125">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="98995-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="98995-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="98995-126">unknownCount</span></span>|<span data-ttu-id="98995-127">Int32</span><span class="sxs-lookup"><span data-stu-id="98995-127">Int32</span></span>|<span data-ttu-id="98995-128">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="98995-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98995-129">Relações</span><span class="sxs-lookup"><span data-stu-id="98995-129">Relationships</span></span>
<span data-ttu-id="98995-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98995-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98995-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98995-131">JSON Representation</span></span>
<span data-ttu-id="98995-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98995-132">Here is a JSON representation of the resource.</span></span>
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







