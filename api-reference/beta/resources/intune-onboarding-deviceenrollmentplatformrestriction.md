---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6fdb900b9f9ce5c89828e6e945623a766de2041
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697235"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="a6adb-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a6adb-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="a6adb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6adb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6adb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6adb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6adb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6adb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6adb-107">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="a6adb-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="a6adb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6adb-108">Properties</span></span>
|<span data-ttu-id="a6adb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6adb-109">Property</span></span>|<span data-ttu-id="a6adb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6adb-110">Type</span></span>|<span data-ttu-id="a6adb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6adb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6adb-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="a6adb-112">platformBlocked</span></span>|<span data-ttu-id="a6adb-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6adb-113">Boolean</span></span>|<span data-ttu-id="a6adb-114">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="a6adb-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="a6adb-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="a6adb-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="a6adb-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6adb-116">Boolean</span></span>|<span data-ttu-id="a6adb-117">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="a6adb-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="a6adb-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a6adb-118">osMinimumVersion</span></span>|<span data-ttu-id="a6adb-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6adb-119">String</span></span>|<span data-ttu-id="a6adb-120">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="a6adb-120">Min OS version supported</span></span>|
|<span data-ttu-id="a6adb-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a6adb-121">osMaximumVersion</span></span>|<span data-ttu-id="a6adb-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6adb-122">String</span></span>|<span data-ttu-id="a6adb-123">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="a6adb-123">Max OS version supported</span></span>|
|<span data-ttu-id="a6adb-124">blockedManufacturers</span><span class="sxs-lookup"><span data-stu-id="a6adb-124">blockedManufacturers</span></span>|<span data-ttu-id="a6adb-125">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6adb-125">String collection</span></span>|<span data-ttu-id="a6adb-126">Conjunto de fabricantes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="a6adb-126">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6adb-127">Relações</span><span class="sxs-lookup"><span data-stu-id="a6adb-127">Relationships</span></span>
<span data-ttu-id="a6adb-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6adb-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6adb-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6adb-129">JSON Representation</span></span>
<span data-ttu-id="a6adb-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6adb-130">Here is a JSON representation of the resource.</span></span>
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





