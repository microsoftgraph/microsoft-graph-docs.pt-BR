---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bf67d9b39462a11286420a6cd6aa79f2e45fb246
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779622"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="4767f-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4767f-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="4767f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4767f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4767f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4767f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4767f-106">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="4767f-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="4767f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4767f-107">Properties</span></span>
|<span data-ttu-id="4767f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4767f-108">Property</span></span>|<span data-ttu-id="4767f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4767f-109">Type</span></span>|<span data-ttu-id="4767f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4767f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4767f-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="4767f-111">platformBlocked</span></span>|<span data-ttu-id="4767f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="4767f-112">Boolean</span></span>|<span data-ttu-id="4767f-113">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="4767f-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="4767f-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="4767f-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="4767f-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="4767f-115">Boolean</span></span>|<span data-ttu-id="4767f-116">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="4767f-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="4767f-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4767f-117">osMinimumVersion</span></span>|<span data-ttu-id="4767f-118">String</span><span class="sxs-lookup"><span data-stu-id="4767f-118">String</span></span>|<span data-ttu-id="4767f-119">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="4767f-119">Min OS version supported</span></span>|
|<span data-ttu-id="4767f-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4767f-120">osMaximumVersion</span></span>|<span data-ttu-id="4767f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4767f-121">String</span></span>|<span data-ttu-id="4767f-122">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="4767f-122">Max OS version supported</span></span>|
|<span data-ttu-id="4767f-123">blockedManufacturers</span><span class="sxs-lookup"><span data-stu-id="4767f-123">blockedManufacturers</span></span>|<span data-ttu-id="4767f-124">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4767f-124">String collection</span></span>|<span data-ttu-id="4767f-125">Conjunto de fabricantes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4767f-125">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4767f-126">Relações</span><span class="sxs-lookup"><span data-stu-id="4767f-126">Relationships</span></span>
<span data-ttu-id="4767f-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4767f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4767f-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4767f-128">JSON Representation</span></span>
<span data-ttu-id="4767f-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4767f-129">Here is a JSON representation of the resource.</span></span>
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



