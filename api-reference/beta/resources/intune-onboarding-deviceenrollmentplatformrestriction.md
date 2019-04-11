---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8ba3306c5a4af4dfbb8b97e4d4794b917ebbf64
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806451"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="a8cb4-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="a8cb4-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="a8cb4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8cb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8cb4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8cb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8cb4-106">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="a8cb4-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="a8cb4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8cb4-107">Properties</span></span>
|<span data-ttu-id="a8cb4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8cb4-108">Property</span></span>|<span data-ttu-id="a8cb4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8cb4-109">Type</span></span>|<span data-ttu-id="a8cb4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8cb4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8cb4-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="a8cb4-111">platformBlocked</span></span>|<span data-ttu-id="a8cb4-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="a8cb4-112">Boolean</span></span>|<span data-ttu-id="a8cb4-113">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="a8cb4-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="a8cb4-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="a8cb4-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="a8cb4-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="a8cb4-115">Boolean</span></span>|<span data-ttu-id="a8cb4-116">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="a8cb4-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="a8cb4-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a8cb4-117">osMinimumVersion</span></span>|<span data-ttu-id="a8cb4-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8cb4-118">String</span></span>|<span data-ttu-id="a8cb4-119">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="a8cb4-119">Min OS version supported</span></span>|
|<span data-ttu-id="a8cb4-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a8cb4-120">osMaximumVersion</span></span>|<span data-ttu-id="a8cb4-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8cb4-121">String</span></span>|<span data-ttu-id="a8cb4-122">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="a8cb4-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8cb4-123">Relações</span><span class="sxs-lookup"><span data-stu-id="a8cb4-123">Relationships</span></span>
<span data-ttu-id="a8cb4-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a8cb4-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8cb4-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8cb4-125">JSON Representation</span></span>
<span data-ttu-id="a8cb4-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8cb4-126">Here is a JSON representation of the resource.</span></span>
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





