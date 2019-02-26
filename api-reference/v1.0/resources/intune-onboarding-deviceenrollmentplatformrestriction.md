---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 306f280928c843b596c57e7bdab454fd138851cc
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260834"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="e299e-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="e299e-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="e299e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e299e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e299e-105">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="e299e-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="e299e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e299e-106">Properties</span></span>
|<span data-ttu-id="e299e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e299e-107">Property</span></span>|<span data-ttu-id="e299e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e299e-108">Type</span></span>|<span data-ttu-id="e299e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e299e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e299e-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="e299e-110">platformBlocked</span></span>|<span data-ttu-id="e299e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="e299e-111">Boolean</span></span>|<span data-ttu-id="e299e-112">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="e299e-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="e299e-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="e299e-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="e299e-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="e299e-114">Boolean</span></span>|<span data-ttu-id="e299e-115">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="e299e-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="e299e-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e299e-116">osMinimumVersion</span></span>|<span data-ttu-id="e299e-117">String</span><span class="sxs-lookup"><span data-stu-id="e299e-117">String</span></span>|<span data-ttu-id="e299e-118">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="e299e-118">Min OS version supported</span></span>|
|<span data-ttu-id="e299e-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e299e-119">osMaximumVersion</span></span>|<span data-ttu-id="e299e-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e299e-120">String</span></span>|<span data-ttu-id="e299e-121">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="e299e-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="e299e-122">Relações</span><span class="sxs-lookup"><span data-stu-id="e299e-122">Relationships</span></span>
<span data-ttu-id="e299e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e299e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e299e-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e299e-124">JSON Representation</span></span>
<span data-ttu-id="e299e-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e299e-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```



