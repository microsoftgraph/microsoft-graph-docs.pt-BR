---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0bf4748d8dc083fe03b55b5ee88062ebb429f639
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422856"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="4504e-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="4504e-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="4504e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4504e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4504e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4504e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4504e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4504e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4504e-107">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="4504e-107">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="4504e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4504e-108">Properties</span></span>
|<span data-ttu-id="4504e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4504e-109">Property</span></span>|<span data-ttu-id="4504e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4504e-110">Type</span></span>|<span data-ttu-id="4504e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4504e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4504e-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="4504e-112">platformBlocked</span></span>|<span data-ttu-id="4504e-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="4504e-113">Boolean</span></span>|<span data-ttu-id="4504e-114">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="4504e-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="4504e-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="4504e-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="4504e-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="4504e-116">Boolean</span></span>|<span data-ttu-id="4504e-117">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="4504e-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="4504e-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4504e-118">osMinimumVersion</span></span>|<span data-ttu-id="4504e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4504e-119">String</span></span>|<span data-ttu-id="4504e-120">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="4504e-120">Min OS version supported</span></span>|
|<span data-ttu-id="4504e-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4504e-121">osMaximumVersion</span></span>|<span data-ttu-id="4504e-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4504e-122">String</span></span>|<span data-ttu-id="4504e-123">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="4504e-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="4504e-124">Relações</span><span class="sxs-lookup"><span data-stu-id="4504e-124">Relationships</span></span>
<span data-ttu-id="4504e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4504e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4504e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4504e-126">JSON Representation</span></span>
<span data-ttu-id="4504e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4504e-127">Here is a JSON representation of the resource.</span></span>
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




