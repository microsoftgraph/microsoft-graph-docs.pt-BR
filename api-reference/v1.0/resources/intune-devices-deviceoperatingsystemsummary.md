---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
ms.openlocfilehash: 1a543f21d1f82b9f2bee0f004d3b8fab88c863b0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005722"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="70565-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="70565-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="70565-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="70565-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70565-105">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="70565-105">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="70565-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70565-106">Properties</span></span>
|<span data-ttu-id="70565-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70565-107">Property</span></span>|<span data-ttu-id="70565-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="70565-108">Type</span></span>|<span data-ttu-id="70565-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="70565-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70565-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="70565-110">androidCount</span></span>|<span data-ttu-id="70565-111">Int32</span><span class="sxs-lookup"><span data-stu-id="70565-111">Int32</span></span>|<span data-ttu-id="70565-112">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="70565-112">Number of android device count.</span></span>|
|<span data-ttu-id="70565-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="70565-113">iosCount</span></span>|<span data-ttu-id="70565-114">Int32</span><span class="sxs-lookup"><span data-stu-id="70565-114">Int32</span></span>|<span data-ttu-id="70565-115">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="70565-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="70565-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="70565-116">macOSCount</span></span>|<span data-ttu-id="70565-117">Int32</span><span class="sxs-lookup"><span data-stu-id="70565-117">Int32</span></span>|<span data-ttu-id="70565-118">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="70565-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="70565-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="70565-119">windowsMobileCount</span></span>|<span data-ttu-id="70565-120">Int32</span><span class="sxs-lookup"><span data-stu-id="70565-120">Int32</span></span>|<span data-ttu-id="70565-121">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="70565-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="70565-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="70565-122">windowsCount</span></span>|<span data-ttu-id="70565-123">Int32</span><span class="sxs-lookup"><span data-stu-id="70565-123">Int32</span></span>|<span data-ttu-id="70565-124">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="70565-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="70565-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="70565-125">unknownCount</span></span>|<span data-ttu-id="70565-126">Int32</span><span class="sxs-lookup"><span data-stu-id="70565-126">Int32</span></span>|<span data-ttu-id="70565-127">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="70565-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70565-128">Relações</span><span class="sxs-lookup"><span data-stu-id="70565-128">Relationships</span></span>
<span data-ttu-id="70565-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70565-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="70565-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70565-130">JSON Representation</span></span>
<span data-ttu-id="70565-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70565-131">Here is a JSON representation of the resource.</span></span>
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



