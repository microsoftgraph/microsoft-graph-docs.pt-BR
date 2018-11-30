---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
ms.openlocfilehash: 13224e18f117f13a6f7c7090d1aa9cb2686350c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040912"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="712db-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="712db-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="712db-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="712db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="712db-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="712db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="712db-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="712db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="712db-107">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="712db-107">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="712db-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="712db-108">Properties</span></span>
|<span data-ttu-id="712db-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="712db-109">Property</span></span>|<span data-ttu-id="712db-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="712db-110">Type</span></span>|<span data-ttu-id="712db-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="712db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="712db-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="712db-112">androidCount</span></span>|<span data-ttu-id="712db-113">Int32</span><span class="sxs-lookup"><span data-stu-id="712db-113">Int32</span></span>|<span data-ttu-id="712db-114">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="712db-114">Number of android device count.</span></span>|
|<span data-ttu-id="712db-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="712db-115">iosCount</span></span>|<span data-ttu-id="712db-116">Int32</span><span class="sxs-lookup"><span data-stu-id="712db-116">Int32</span></span>|<span data-ttu-id="712db-117">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="712db-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="712db-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="712db-118">macOSCount</span></span>|<span data-ttu-id="712db-119">Int32</span><span class="sxs-lookup"><span data-stu-id="712db-119">Int32</span></span>|<span data-ttu-id="712db-120">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="712db-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="712db-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="712db-121">windowsMobileCount</span></span>|<span data-ttu-id="712db-122">Int32</span><span class="sxs-lookup"><span data-stu-id="712db-122">Int32</span></span>|<span data-ttu-id="712db-123">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="712db-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="712db-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="712db-124">windowsCount</span></span>|<span data-ttu-id="712db-125">Int32</span><span class="sxs-lookup"><span data-stu-id="712db-125">Int32</span></span>|<span data-ttu-id="712db-126">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="712db-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="712db-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="712db-127">unknownCount</span></span>|<span data-ttu-id="712db-128">Int32</span><span class="sxs-lookup"><span data-stu-id="712db-128">Int32</span></span>|<span data-ttu-id="712db-129">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="712db-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="712db-130">Relações</span><span class="sxs-lookup"><span data-stu-id="712db-130">Relationships</span></span>
<span data-ttu-id="712db-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="712db-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="712db-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="712db-132">JSON Representation</span></span>
<span data-ttu-id="712db-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="712db-133">Here is a JSON representation of the resource.</span></span>
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





