---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26f29427dfe863ed1b89eaef5025655dc07430fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636592"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="62d7b-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="62d7b-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="62d7b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62d7b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62d7b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62d7b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62d7b-106">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="62d7b-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="62d7b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62d7b-107">Properties</span></span>
|<span data-ttu-id="62d7b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62d7b-108">Property</span></span>|<span data-ttu-id="62d7b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="62d7b-109">Type</span></span>|<span data-ttu-id="62d7b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="62d7b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62d7b-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="62d7b-111">platformBlocked</span></span>|<span data-ttu-id="62d7b-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="62d7b-112">Boolean</span></span>|<span data-ttu-id="62d7b-113">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="62d7b-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="62d7b-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="62d7b-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="62d7b-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="62d7b-115">Boolean</span></span>|<span data-ttu-id="62d7b-116">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="62d7b-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="62d7b-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="62d7b-117">osMinimumVersion</span></span>|<span data-ttu-id="62d7b-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62d7b-118">String</span></span>|<span data-ttu-id="62d7b-119">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="62d7b-119">Min OS version supported</span></span>|
|<span data-ttu-id="62d7b-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="62d7b-120">osMaximumVersion</span></span>|<span data-ttu-id="62d7b-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62d7b-121">String</span></span>|<span data-ttu-id="62d7b-122">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="62d7b-122">Max OS version supported</span></span>|
|<span data-ttu-id="62d7b-123">blockedManufacturers</span><span class="sxs-lookup"><span data-stu-id="62d7b-123">blockedManufacturers</span></span>|<span data-ttu-id="62d7b-124">String collection</span><span class="sxs-lookup"><span data-stu-id="62d7b-124">String collection</span></span>|<span data-ttu-id="62d7b-125">Conjunto de fabricantes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="62d7b-125">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62d7b-126">Relações</span><span class="sxs-lookup"><span data-stu-id="62d7b-126">Relationships</span></span>
<span data-ttu-id="62d7b-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62d7b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62d7b-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62d7b-128">JSON Representation</span></span>
<span data-ttu-id="62d7b-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62d7b-129">Here is a JSON representation of the resource.</span></span>
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



