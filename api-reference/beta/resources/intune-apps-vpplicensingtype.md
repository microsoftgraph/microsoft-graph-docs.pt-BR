---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12cf34dd1ecf2bdad349bf5f20125b8484e22826
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707952"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="694e0-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="694e0-103">vppLicensingType resource type</span></span>

<span data-ttu-id="694e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="694e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="694e0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="694e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="694e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="694e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="694e0-107">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="694e0-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="694e0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="694e0-108">Properties</span></span>
|<span data-ttu-id="694e0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="694e0-109">Property</span></span>|<span data-ttu-id="694e0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="694e0-110">Type</span></span>|<span data-ttu-id="694e0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="694e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="694e0-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="694e0-112">supportUserLicensing</span></span>|<span data-ttu-id="694e0-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="694e0-113">Boolean</span></span>|<span data-ttu-id="694e0-114">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="694e0-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="694e0-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="694e0-115">supportDeviceLicensing</span></span>|<span data-ttu-id="694e0-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="694e0-116">Boolean</span></span>|<span data-ttu-id="694e0-117">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="694e0-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="694e0-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="694e0-118">supportsUserLicensing</span></span>|<span data-ttu-id="694e0-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="694e0-119">Boolean</span></span>|<span data-ttu-id="694e0-120">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="694e0-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="694e0-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="694e0-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="694e0-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="694e0-122">Boolean</span></span>|<span data-ttu-id="694e0-123">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="694e0-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="694e0-124">Relações</span><span class="sxs-lookup"><span data-stu-id="694e0-124">Relationships</span></span>
<span data-ttu-id="694e0-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="694e0-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="694e0-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="694e0-126">JSON Representation</span></span>
<span data-ttu-id="694e0-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="694e0-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```





