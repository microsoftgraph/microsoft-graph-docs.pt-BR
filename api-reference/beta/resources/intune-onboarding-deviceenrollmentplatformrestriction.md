---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed769c1e6550584688324f4bfdf2db772feae19c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524185"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="c07c1-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="c07c1-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="c07c1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c07c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c07c1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c07c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c07c1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c07c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c07c1-107">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="c07c1-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="c07c1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c07c1-108">Properties</span></span>
|<span data-ttu-id="c07c1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c07c1-109">Property</span></span>|<span data-ttu-id="c07c1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c07c1-110">Type</span></span>|<span data-ttu-id="c07c1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c07c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c07c1-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="c07c1-112">platformBlocked</span></span>|<span data-ttu-id="c07c1-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c07c1-113">Boolean</span></span>|<span data-ttu-id="c07c1-114">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="c07c1-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="c07c1-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="c07c1-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="c07c1-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="c07c1-116">Boolean</span></span>|<span data-ttu-id="c07c1-117">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="c07c1-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="c07c1-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c07c1-118">osMinimumVersion</span></span>|<span data-ttu-id="c07c1-119">String</span><span class="sxs-lookup"><span data-stu-id="c07c1-119">String</span></span>|<span data-ttu-id="c07c1-120">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="c07c1-120">Min OS version supported</span></span>|
|<span data-ttu-id="c07c1-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c07c1-121">osMaximumVersion</span></span>|<span data-ttu-id="c07c1-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07c1-122">String</span></span>|<span data-ttu-id="c07c1-123">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="c07c1-123">Max OS version supported</span></span>|
|<span data-ttu-id="c07c1-124">blockedManufacturers</span><span class="sxs-lookup"><span data-stu-id="c07c1-124">blockedManufacturers</span></span>|<span data-ttu-id="c07c1-125">String collection</span><span class="sxs-lookup"><span data-stu-id="c07c1-125">String collection</span></span>|<span data-ttu-id="c07c1-126">Conjunto de fabricantes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="c07c1-126">Collection of blocked Manufacturers.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c07c1-127">Relações</span><span class="sxs-lookup"><span data-stu-id="c07c1-127">Relationships</span></span>
<span data-ttu-id="c07c1-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c07c1-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c07c1-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c07c1-129">JSON Representation</span></span>
<span data-ttu-id="c07c1-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c07c1-130">Here is a JSON representation of the resource.</span></span>
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



