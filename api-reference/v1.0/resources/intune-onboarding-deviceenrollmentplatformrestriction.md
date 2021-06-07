---
title: Tipo de recurso deviceEnrollmentPlatformRestriction
description: Restrições de registro específicas de plataformas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02978735f15ce036c8ffbc81340d965d67a21ce8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751612"
---
# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="8aec9-103">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8aec9-103">deviceEnrollmentPlatformRestriction resource type</span></span>

<span data-ttu-id="8aec9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aec9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8aec9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8aec9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8aec9-106">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="8aec9-106">Platform specific enrollment restrictions</span></span>

## <a name="properties"></a><span data-ttu-id="8aec9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8aec9-107">Properties</span></span>
|<span data-ttu-id="8aec9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8aec9-108">Property</span></span>|<span data-ttu-id="8aec9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aec9-109">Type</span></span>|<span data-ttu-id="8aec9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aec9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aec9-111">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="8aec9-111">platformBlocked</span></span>|<span data-ttu-id="8aec9-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aec9-112">Boolean</span></span>|<span data-ttu-id="8aec9-113">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="8aec9-113">Block the platform from enrolling</span></span>|
|<span data-ttu-id="8aec9-114">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="8aec9-114">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="8aec9-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="8aec9-115">Boolean</span></span>|<span data-ttu-id="8aec9-116">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="8aec9-116">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="8aec9-117">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8aec9-117">osMinimumVersion</span></span>|<span data-ttu-id="8aec9-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aec9-118">String</span></span>|<span data-ttu-id="8aec9-119">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="8aec9-119">Min OS version supported</span></span>|
|<span data-ttu-id="8aec9-120">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8aec9-120">osMaximumVersion</span></span>|<span data-ttu-id="8aec9-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aec9-121">String</span></span>|<span data-ttu-id="8aec9-122">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="8aec9-122">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="8aec9-123">Relações</span><span class="sxs-lookup"><span data-stu-id="8aec9-123">Relationships</span></span>
<span data-ttu-id="8aec9-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8aec9-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8aec9-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8aec9-125">JSON Representation</span></span>
<span data-ttu-id="8aec9-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8aec9-126">Here is a JSON representation of the resource.</span></span>
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




