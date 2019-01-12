---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e5189b286de61375715944c5ac979d847392a18c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917759"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="1c057-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="1c057-103">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="1c057-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1c057-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c057-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1c057-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c057-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1c057-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c057-107">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="1c057-107">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="1c057-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c057-108">Properties</span></span>
|<span data-ttu-id="1c057-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c057-109">Property</span></span>|<span data-ttu-id="1c057-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c057-110">Type</span></span>|<span data-ttu-id="1c057-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c057-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c057-112">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="1c057-112">platformBlocked</span></span>|<span data-ttu-id="1c057-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c057-113">Boolean</span></span>|<span data-ttu-id="1c057-114">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="1c057-114">Block the platform from enrolling</span></span>|
|<span data-ttu-id="1c057-115">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="1c057-115">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="1c057-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c057-116">Boolean</span></span>|<span data-ttu-id="1c057-117">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="1c057-117">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="1c057-118">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1c057-118">osMinimumVersion</span></span>|<span data-ttu-id="1c057-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c057-119">String</span></span>|<span data-ttu-id="1c057-120">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="1c057-120">Min OS version supported</span></span>|
|<span data-ttu-id="1c057-121">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1c057-121">osMaximumVersion</span></span>|<span data-ttu-id="1c057-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c057-122">String</span></span>|<span data-ttu-id="1c057-123">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="1c057-123">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c057-124">Relações</span><span class="sxs-lookup"><span data-stu-id="1c057-124">Relationships</span></span>
<span data-ttu-id="1c057-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c057-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1c057-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c057-126">JSON Representation</span></span>
<span data-ttu-id="1c057-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c057-127">Here is a JSON representation of the resource.</span></span>
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





