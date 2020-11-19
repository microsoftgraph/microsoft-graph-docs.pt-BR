---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05105eec5b3b870ee608d0b47861d1eaddae8965
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301274"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="70963-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="70963-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="70963-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70963-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70963-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70963-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70963-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70963-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70963-107">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="70963-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="70963-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70963-108">Properties</span></span>
|<span data-ttu-id="70963-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70963-109">Property</span></span>|<span data-ttu-id="70963-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="70963-110">Type</span></span>|<span data-ttu-id="70963-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="70963-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70963-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="70963-112">platformBlocked</span></span>|<span data-ttu-id="70963-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="70963-113">Boolean</span></span>|<span data-ttu-id="70963-114">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="70963-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="70963-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="70963-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="70963-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="70963-116">Boolean</span></span>|<span data-ttu-id="70963-117">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="70963-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="70963-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="70963-118">osMinimumVersion</span></span>|<span data-ttu-id="70963-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70963-119">String</span></span>|<span data-ttu-id="70963-120">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="70963-120">Min OS version supported</span></span>|
|<span data-ttu-id="70963-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="70963-121">osMaximumVersion</span></span>|<span data-ttu-id="70963-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70963-122">String</span></span>|<span data-ttu-id="70963-123">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="70963-123">Max OS version supported</span></span>|
|<span data-ttu-id="70963-124">blockedManufacturers</span><span class="sxs-lookup"><span data-stu-id="70963-124">blockedManufacturers</span></span>|<span data-ttu-id="70963-125">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="70963-125">String collection</span></span>|<span data-ttu-id="70963-126">Conjunto de fabricantes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="70963-126">Collection of blocked Manufacturers.</span></span>|
|<span data-ttu-id="70963-127">blockedSkus</span><span class="sxs-lookup"><span data-stu-id="70963-127">blockedSkus</span></span>|<span data-ttu-id="70963-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="70963-128">String collection</span></span>|<span data-ttu-id="70963-129">Conjunto de SKUs bloqueados.</span><span class="sxs-lookup"><span data-stu-id="70963-129">Collection of blocked Skus.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70963-130">Relações</span><span class="sxs-lookup"><span data-stu-id="70963-130">Relationships</span></span>
<span data-ttu-id="70963-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70963-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70963-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70963-132">JSON Representation</span></span>
<span data-ttu-id="70963-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70963-133">Here is a JSON representation of the resource.</span></span>
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
  ],
  "blockedSkus": [
    "String"
  ]
}
```




