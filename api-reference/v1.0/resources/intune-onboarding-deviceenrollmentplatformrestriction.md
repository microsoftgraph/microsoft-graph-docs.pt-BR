---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 306f280928c843b596c57e7bdab454fd138851cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571195"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="f30e0-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="f30e0-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="f30e0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f30e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f30e0-105">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="f30e0-105">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="f30e0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f30e0-106">Properties</span></span>
|<span data-ttu-id="f30e0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f30e0-107">Property</span></span>|<span data-ttu-id="f30e0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f30e0-108">Type</span></span>|<span data-ttu-id="f30e0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f30e0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f30e0-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="f30e0-110">platformBlocked</span></span>|<span data-ttu-id="f30e0-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="f30e0-111">Boolean</span></span>|<span data-ttu-id="f30e0-112">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="f30e0-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="f30e0-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="f30e0-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="f30e0-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="f30e0-114">Boolean</span></span>|<span data-ttu-id="f30e0-115">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="f30e0-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="f30e0-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f30e0-116">osMinimumVersion</span></span>|<span data-ttu-id="f30e0-117">String</span><span class="sxs-lookup"><span data-stu-id="f30e0-117">String</span></span>|<span data-ttu-id="f30e0-118">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="f30e0-118">Min OS version supported</span></span>|
|<span data-ttu-id="f30e0-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f30e0-119">osMaximumVersion</span></span>|<span data-ttu-id="f30e0-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f30e0-120">String</span></span>|<span data-ttu-id="f30e0-121">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="f30e0-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="f30e0-122">Relações</span><span class="sxs-lookup"><span data-stu-id="f30e0-122">Relationships</span></span>
<span data-ttu-id="f30e0-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f30e0-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f30e0-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f30e0-124">JSON Representation</span></span>
<span data-ttu-id="f30e0-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f30e0-125">Here is a JSON representation of the resource.</span></span>
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



