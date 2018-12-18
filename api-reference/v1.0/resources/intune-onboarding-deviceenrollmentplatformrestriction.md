---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: tfitzmac
ms.openlocfilehash: cccac8240457ffe2b5c27475e8ac9e8fb83200ea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329383"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="8da20-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8da20-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="8da20-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8da20-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8da20-105">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="8da20-105">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="8da20-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8da20-106">Properties</span></span>
|<span data-ttu-id="8da20-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8da20-107">Property</span></span>|<span data-ttu-id="8da20-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8da20-108">Type</span></span>|<span data-ttu-id="8da20-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8da20-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8da20-110">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="8da20-110">platformBlocked</span></span>|<span data-ttu-id="8da20-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="8da20-111">Boolean</span></span>|<span data-ttu-id="8da20-112">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="8da20-112">Block the platform from enrolling</span></span>|
|<span data-ttu-id="8da20-113">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="8da20-113">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="8da20-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="8da20-114">Boolean</span></span>|<span data-ttu-id="8da20-115">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="8da20-115">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="8da20-116">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8da20-116">osMinimumVersion</span></span>|<span data-ttu-id="8da20-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8da20-117">String</span></span>|<span data-ttu-id="8da20-118">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="8da20-118">Min OS version supported</span></span>|
|<span data-ttu-id="8da20-119">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8da20-119">osMaximumVersion</span></span>|<span data-ttu-id="8da20-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8da20-120">String</span></span>|<span data-ttu-id="8da20-121">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="8da20-121">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="8da20-122">Relações</span><span class="sxs-lookup"><span data-stu-id="8da20-122">Relationships</span></span>
<span data-ttu-id="8da20-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8da20-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8da20-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8da20-124">JSON Representation</span></span>
<span data-ttu-id="8da20-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8da20-125">Here is a JSON representation of the resource.</span></span>
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



