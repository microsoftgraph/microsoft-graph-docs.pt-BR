---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c621eb9fc0b90e752d46b8ab1a3d75a927c16051
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086539"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="c43a8-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="c43a8-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="c43a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c43a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c43a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c43a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c43a8-106">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="c43a8-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="c43a8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c43a8-107">Properties</span></span>
|<span data-ttu-id="c43a8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c43a8-108">Property</span></span>|<span data-ttu-id="c43a8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c43a8-109">Type</span></span>|<span data-ttu-id="c43a8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c43a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c43a8-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="c43a8-111">platformBlocked</span></span>|<span data-ttu-id="c43a8-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="c43a8-112">Boolean</span></span>|<span data-ttu-id="c43a8-113">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="c43a8-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="c43a8-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="c43a8-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="c43a8-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="c43a8-115">Boolean</span></span>|<span data-ttu-id="c43a8-116">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="c43a8-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="c43a8-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c43a8-117">osMinimumVersion</span></span>|<span data-ttu-id="c43a8-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c43a8-118">String</span></span>|<span data-ttu-id="c43a8-119">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="c43a8-119">Min OS version supported</span></span>|
|<span data-ttu-id="c43a8-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c43a8-120">osMaximumVersion</span></span>|<span data-ttu-id="c43a8-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c43a8-121">String</span></span>|<span data-ttu-id="c43a8-122">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="c43a8-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="c43a8-123">Relações</span><span class="sxs-lookup"><span data-stu-id="c43a8-123">Relationships</span></span>
<span data-ttu-id="c43a8-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c43a8-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c43a8-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c43a8-125">JSON Representation</span></span>
<span data-ttu-id="c43a8-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c43a8-126">Here is a JSON representation of the resource.</span></span>
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









