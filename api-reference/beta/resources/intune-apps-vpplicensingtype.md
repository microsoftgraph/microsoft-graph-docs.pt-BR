---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 812cbdc203b09422f8a2cddac205d59f8c762a34
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949707"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="8c354-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="8c354-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="8c354-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c354-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c354-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c354-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c354-106">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="8c354-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="8c354-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c354-107">Properties</span></span>
|<span data-ttu-id="8c354-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c354-108">Property</span></span>|<span data-ttu-id="8c354-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c354-109">Type</span></span>|<span data-ttu-id="8c354-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c354-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c354-111">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="8c354-111">supportUserLicensing</span></span>|<span data-ttu-id="8c354-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c354-112">Boolean</span></span>|<span data-ttu-id="8c354-113">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="8c354-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="8c354-114">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8c354-114">supportDeviceLicensing</span></span>|<span data-ttu-id="8c354-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c354-115">Boolean</span></span>|<span data-ttu-id="8c354-116">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c354-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="8c354-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="8c354-117">supportsUserLicensing</span></span>|<span data-ttu-id="8c354-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c354-118">Boolean</span></span>|<span data-ttu-id="8c354-119">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="8c354-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="8c354-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8c354-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="8c354-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c354-121">Boolean</span></span>|<span data-ttu-id="8c354-122">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8c354-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c354-123">Relações</span><span class="sxs-lookup"><span data-stu-id="8c354-123">Relationships</span></span>
<span data-ttu-id="8c354-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c354-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c354-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c354-125">JSON Representation</span></span>
<span data-ttu-id="8c354-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c354-126">Here is a JSON representation of the resource.</span></span>
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




