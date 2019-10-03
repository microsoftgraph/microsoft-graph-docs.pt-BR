---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: edf64c6aaa2a9745b28543bd3dc3a458b7d8869e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367235"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="4648d-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4648d-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="4648d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4648d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4648d-105">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="4648d-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="4648d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4648d-106">Properties</span></span>
|<span data-ttu-id="4648d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4648d-107">Property</span></span>|<span data-ttu-id="4648d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4648d-108">Type</span></span>|<span data-ttu-id="4648d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4648d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4648d-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="4648d-110">platformBlocked</span></span>|<span data-ttu-id="4648d-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="4648d-111">Boolean</span></span>|<span data-ttu-id="4648d-112">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="4648d-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="4648d-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="4648d-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="4648d-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="4648d-114">Boolean</span></span>|<span data-ttu-id="4648d-115">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="4648d-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="4648d-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4648d-116">osMinimumVersion</span></span>|<span data-ttu-id="4648d-117">String</span><span class="sxs-lookup"><span data-stu-id="4648d-117">String</span></span>|<span data-ttu-id="4648d-118">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="4648d-118">Min OS version supported</span></span>|
|<span data-ttu-id="4648d-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4648d-119">osMaximumVersion</span></span>|<span data-ttu-id="4648d-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4648d-120">String</span></span>|<span data-ttu-id="4648d-121">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="4648d-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="4648d-122">Relações</span><span class="sxs-lookup"><span data-stu-id="4648d-122">Relationships</span></span>
<span data-ttu-id="4648d-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4648d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4648d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4648d-124">JSON Representation</span></span>
<span data-ttu-id="4648d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4648d-125">Here is a JSON representation of the resource.</span></span>
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




