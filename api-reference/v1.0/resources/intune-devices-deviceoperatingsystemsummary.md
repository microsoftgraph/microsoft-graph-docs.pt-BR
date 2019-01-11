---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b4b53d7c7260e58458995093bbea17df5464e704
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846071"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="d8e05-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="d8e05-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="d8e05-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d8e05-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8e05-105">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8e05-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="d8e05-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8e05-106">Properties</span></span>
|<span data-ttu-id="d8e05-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8e05-107">Property</span></span>|<span data-ttu-id="d8e05-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8e05-108">Type</span></span>|<span data-ttu-id="d8e05-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8e05-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e05-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="d8e05-110">androidCount</span></span>|<span data-ttu-id="d8e05-111">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e05-111">Int32</span></span>|<span data-ttu-id="d8e05-112">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="d8e05-112">Number of android device count.</span></span>|
|<span data-ttu-id="d8e05-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="d8e05-113">iosCount</span></span>|<span data-ttu-id="d8e05-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e05-114">Int32</span></span>|<span data-ttu-id="d8e05-115">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="d8e05-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="d8e05-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="d8e05-116">macOSCount</span></span>|<span data-ttu-id="d8e05-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e05-117">Int32</span></span>|<span data-ttu-id="d8e05-118">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="d8e05-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="d8e05-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="d8e05-119">windowsMobileCount</span></span>|<span data-ttu-id="d8e05-120">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e05-120">Int32</span></span>|<span data-ttu-id="d8e05-121">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="d8e05-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="d8e05-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="d8e05-122">windowsCount</span></span>|<span data-ttu-id="d8e05-123">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e05-123">Int32</span></span>|<span data-ttu-id="d8e05-124">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="d8e05-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="d8e05-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="d8e05-125">unknownCount</span></span>|<span data-ttu-id="d8e05-126">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e05-126">Int32</span></span>|<span data-ttu-id="d8e05-127">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="d8e05-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8e05-128">Relações</span><span class="sxs-lookup"><span data-stu-id="d8e05-128">Relationships</span></span>
<span data-ttu-id="d8e05-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8e05-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d8e05-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8e05-130">JSON Representation</span></span>
<span data-ttu-id="d8e05-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8e05-131">Here is a JSON representation of the resource.</span></span>
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



