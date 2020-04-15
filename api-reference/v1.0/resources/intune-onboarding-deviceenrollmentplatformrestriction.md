---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 248127b41ca999ceba27f077391a7afa3f4bfbae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459555"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="06b63-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="06b63-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="06b63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06b63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06b63-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06b63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06b63-106">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="06b63-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="06b63-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06b63-107">Properties</span></span>
|<span data-ttu-id="06b63-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06b63-108">Property</span></span>|<span data-ttu-id="06b63-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="06b63-109">Type</span></span>|<span data-ttu-id="06b63-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06b63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06b63-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="06b63-111">platformBlocked</span></span>|<span data-ttu-id="06b63-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="06b63-112">Boolean</span></span>|<span data-ttu-id="06b63-113">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="06b63-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="06b63-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="06b63-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="06b63-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="06b63-115">Boolean</span></span>|<span data-ttu-id="06b63-116">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="06b63-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="06b63-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="06b63-117">osMinimumVersion</span></span>|<span data-ttu-id="06b63-118">String</span><span class="sxs-lookup"><span data-stu-id="06b63-118">String</span></span>|<span data-ttu-id="06b63-119">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="06b63-119">Min OS version supported</span></span>|
|<span data-ttu-id="06b63-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="06b63-120">osMaximumVersion</span></span>|<span data-ttu-id="06b63-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06b63-121">String</span></span>|<span data-ttu-id="06b63-122">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="06b63-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="06b63-123">Relações</span><span class="sxs-lookup"><span data-stu-id="06b63-123">Relationships</span></span>
<span data-ttu-id="06b63-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06b63-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06b63-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06b63-125">JSON Representation</span></span>
<span data-ttu-id="06b63-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06b63-126">Here is a JSON representation of the resource.</span></span>
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







