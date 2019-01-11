---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ce30b9ff24067fb2bfec17ad85d3c8827cc6b798
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815999"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="89b55-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="89b55-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="89b55-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="89b55-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89b55-105">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="89b55-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="89b55-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89b55-106">Properties</span></span>
|<span data-ttu-id="89b55-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89b55-107">Property</span></span>|<span data-ttu-id="89b55-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="89b55-108">Type</span></span>|<span data-ttu-id="89b55-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="89b55-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89b55-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="89b55-110">platformBlocked</span></span>|<span data-ttu-id="89b55-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="89b55-111">Boolean</span></span>|<span data-ttu-id="89b55-112">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="89b55-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="89b55-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="89b55-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="89b55-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="89b55-114">Boolean</span></span>|<span data-ttu-id="89b55-115">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="89b55-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="89b55-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="89b55-116">osMinimumVersion</span></span>|<span data-ttu-id="89b55-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89b55-117">String</span></span>|<span data-ttu-id="89b55-118">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="89b55-118">Min OS version supported</span></span>|
|<span data-ttu-id="89b55-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="89b55-119">osMaximumVersion</span></span>|<span data-ttu-id="89b55-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89b55-120">String</span></span>|<span data-ttu-id="89b55-121">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="89b55-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="89b55-122">Relações</span><span class="sxs-lookup"><span data-stu-id="89b55-122">Relationships</span></span>
<span data-ttu-id="89b55-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89b55-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="89b55-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89b55-124">JSON Representation</span></span>
<span data-ttu-id="89b55-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89b55-125">Here is a JSON representation of the resource.</span></span>
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



