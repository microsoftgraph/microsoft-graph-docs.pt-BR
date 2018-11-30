---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
ms.openlocfilehash: 823eecc37dc8ee4536d5cb63213f2bb80ca5138d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039271"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="2916b-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="2916b-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="2916b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2916b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2916b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2916b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2916b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2916b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2916b-107">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="2916b-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="2916b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2916b-108">Properties</span></span>
|<span data-ttu-id="2916b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2916b-109">Property</span></span>|<span data-ttu-id="2916b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2916b-110">Type</span></span>|<span data-ttu-id="2916b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2916b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2916b-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="2916b-112">platformBlocked</span></span>|<span data-ttu-id="2916b-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="2916b-113">Boolean</span></span>|<span data-ttu-id="2916b-114">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="2916b-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="2916b-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="2916b-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="2916b-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="2916b-116">Boolean</span></span>|<span data-ttu-id="2916b-117">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="2916b-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="2916b-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2916b-118">osMinimumVersion</span></span>|<span data-ttu-id="2916b-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2916b-119">String</span></span>|<span data-ttu-id="2916b-120">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="2916b-120">Min OS version supported</span></span>|
|<span data-ttu-id="2916b-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2916b-121">osMaximumVersion</span></span>|<span data-ttu-id="2916b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2916b-122">String</span></span>|<span data-ttu-id="2916b-123">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="2916b-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="2916b-124">Relações</span><span class="sxs-lookup"><span data-stu-id="2916b-124">Relationships</span></span>
<span data-ttu-id="2916b-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2916b-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2916b-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2916b-126">JSON Representation</span></span>
<span data-ttu-id="2916b-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2916b-127">Here is a JSON representation of the resource.</span></span>
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





