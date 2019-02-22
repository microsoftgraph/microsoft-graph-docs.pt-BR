---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eecbc405fd56d21f7be1c7b9bccd5254db89c8d1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140597"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="4d9bd-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4d9bd-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="4d9bd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d9bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d9bd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d9bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d9bd-106">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="4d9bd-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="4d9bd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d9bd-107">Properties</span></span>
|<span data-ttu-id="4d9bd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d9bd-108">Property</span></span>|<span data-ttu-id="4d9bd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d9bd-109">Type</span></span>|<span data-ttu-id="4d9bd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d9bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d9bd-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="4d9bd-111">platformBlocked</span></span>|<span data-ttu-id="4d9bd-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d9bd-112">Boolean</span></span>|<span data-ttu-id="4d9bd-113">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="4d9bd-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="4d9bd-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="4d9bd-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="4d9bd-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d9bd-115">Boolean</span></span>|<span data-ttu-id="4d9bd-116">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="4d9bd-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="4d9bd-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4d9bd-117">osMinimumVersion</span></span>|<span data-ttu-id="4d9bd-118">String</span><span class="sxs-lookup"><span data-stu-id="4d9bd-118">String</span></span>|<span data-ttu-id="4d9bd-119">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="4d9bd-119">Min OS version supported</span></span>|
|<span data-ttu-id="4d9bd-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4d9bd-120">osMaximumVersion</span></span>|<span data-ttu-id="4d9bd-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d9bd-121">String</span></span>|<span data-ttu-id="4d9bd-122">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="4d9bd-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d9bd-123">Relações</span><span class="sxs-lookup"><span data-stu-id="4d9bd-123">Relationships</span></span>
<span data-ttu-id="4d9bd-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4d9bd-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d9bd-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d9bd-125">JSON Representation</span></span>
<span data-ttu-id="4d9bd-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d9bd-126">Here is a JSON representation of the resource.</span></span>
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




