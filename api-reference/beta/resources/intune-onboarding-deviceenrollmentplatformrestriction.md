---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 009485c2051c47209074ae8b938e6b1b06de9eac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843859"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="77c9e-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="77c9e-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="77c9e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="77c9e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77c9e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="77c9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77c9e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="77c9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77c9e-107">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="77c9e-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="77c9e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77c9e-108">Properties</span></span>
|<span data-ttu-id="77c9e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77c9e-109">Property</span></span>|<span data-ttu-id="77c9e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="77c9e-110">Type</span></span>|<span data-ttu-id="77c9e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="77c9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77c9e-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="77c9e-112">platformBlocked</span></span>|<span data-ttu-id="77c9e-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="77c9e-113">Boolean</span></span>|<span data-ttu-id="77c9e-114">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="77c9e-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="77c9e-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="77c9e-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="77c9e-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="77c9e-116">Boolean</span></span>|<span data-ttu-id="77c9e-117">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="77c9e-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="77c9e-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="77c9e-118">osMinimumVersion</span></span>|<span data-ttu-id="77c9e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77c9e-119">String</span></span>|<span data-ttu-id="77c9e-120">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="77c9e-120">Min OS version supported</span></span>|
|<span data-ttu-id="77c9e-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="77c9e-121">osMaximumVersion</span></span>|<span data-ttu-id="77c9e-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77c9e-122">String</span></span>|<span data-ttu-id="77c9e-123">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="77c9e-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="77c9e-124">Relações</span><span class="sxs-lookup"><span data-stu-id="77c9e-124">Relationships</span></span>
<span data-ttu-id="77c9e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77c9e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="77c9e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77c9e-126">JSON Representation</span></span>
<span data-ttu-id="77c9e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77c9e-127">Here is a JSON representation of the resource.</span></span>
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





