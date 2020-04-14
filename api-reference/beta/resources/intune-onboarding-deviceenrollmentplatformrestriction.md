---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ede5fac054b457230a8523539f3bf0f3a72ce4a7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455124"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="65e11-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="65e11-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="65e11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65e11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65e11-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65e11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65e11-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65e11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65e11-107">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="65e11-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="65e11-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65e11-108">Properties</span></span>
|<span data-ttu-id="65e11-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65e11-109">Property</span></span>|<span data-ttu-id="65e11-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="65e11-110">Type</span></span>|<span data-ttu-id="65e11-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="65e11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65e11-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="65e11-112">platformBlocked</span></span>|<span data-ttu-id="65e11-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="65e11-113">Boolean</span></span>|<span data-ttu-id="65e11-114">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="65e11-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="65e11-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="65e11-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="65e11-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="65e11-116">Boolean</span></span>|<span data-ttu-id="65e11-117">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="65e11-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="65e11-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="65e11-118">osMinimumVersion</span></span>|<span data-ttu-id="65e11-119">String</span><span class="sxs-lookup"><span data-stu-id="65e11-119">String</span></span>|<span data-ttu-id="65e11-120">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="65e11-120">Min OS version supported</span></span>|
|<span data-ttu-id="65e11-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="65e11-121">osMaximumVersion</span></span>|<span data-ttu-id="65e11-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65e11-122">String</span></span>|<span data-ttu-id="65e11-123">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="65e11-123">Max OS version supported</span></span>|
|<span data-ttu-id="65e11-124">blockedManufacturers</span><span class="sxs-lookup"><span data-stu-id="65e11-124">blockedManufacturers</span></span>|<span data-ttu-id="65e11-125">Coleção String</span><span class="sxs-lookup"><span data-stu-id="65e11-125">String collection</span></span>|<span data-ttu-id="65e11-126">Conjunto de fabricantes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="65e11-126">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65e11-127">Relações</span><span class="sxs-lookup"><span data-stu-id="65e11-127">Relationships</span></span>
<span data-ttu-id="65e11-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65e11-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65e11-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65e11-129">JSON Representation</span></span>
<span data-ttu-id="65e11-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65e11-130">Here is a JSON representation of the resource.</span></span>
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
  "osMaximumVersion": "String",
  "blockedManufacturers": [
    "String"
  ]
}
```



