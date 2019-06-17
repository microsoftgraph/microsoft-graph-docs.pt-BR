---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0288883ec1deaaecc142aec42f413a4f60a76b5b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993155"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="6f7ed-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="6f7ed-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="6f7ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f7ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f7ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f7ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f7ed-106">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="6f7ed-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="6f7ed-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f7ed-107">Properties</span></span>
|<span data-ttu-id="6f7ed-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f7ed-108">Property</span></span>|<span data-ttu-id="6f7ed-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f7ed-109">Type</span></span>|<span data-ttu-id="6f7ed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f7ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f7ed-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="6f7ed-111">platformBlocked</span></span>|<span data-ttu-id="6f7ed-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f7ed-112">Boolean</span></span>|<span data-ttu-id="6f7ed-113">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="6f7ed-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="6f7ed-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="6f7ed-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="6f7ed-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f7ed-115">Boolean</span></span>|<span data-ttu-id="6f7ed-116">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="6f7ed-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="6f7ed-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6f7ed-117">osMinimumVersion</span></span>|<span data-ttu-id="6f7ed-118">String</span><span class="sxs-lookup"><span data-stu-id="6f7ed-118">String</span></span>|<span data-ttu-id="6f7ed-119">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="6f7ed-119">Min OS version supported</span></span>|
|<span data-ttu-id="6f7ed-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6f7ed-120">osMaximumVersion</span></span>|<span data-ttu-id="6f7ed-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f7ed-121">String</span></span>|<span data-ttu-id="6f7ed-122">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="6f7ed-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f7ed-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6f7ed-123">Relationships</span></span>
<span data-ttu-id="6f7ed-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f7ed-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f7ed-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f7ed-125">JSON Representation</span></span>
<span data-ttu-id="6f7ed-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f7ed-126">Here is a JSON representation of the resource.</span></span>
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





