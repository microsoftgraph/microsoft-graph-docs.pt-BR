---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c04e3fbc7da2a355dc8d5b1e69ad90a6f333a9cf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797693"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="26b62-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="26b62-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="26b62-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26b62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26b62-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26b62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26b62-106">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="26b62-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="26b62-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26b62-107">Properties</span></span>
|<span data-ttu-id="26b62-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26b62-108">Property</span></span>|<span data-ttu-id="26b62-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="26b62-109">Type</span></span>|<span data-ttu-id="26b62-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="26b62-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26b62-111">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="26b62-111">supportUserLicensing</span></span>|<span data-ttu-id="26b62-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b62-112">Boolean</span></span>|<span data-ttu-id="26b62-113">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="26b62-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="26b62-114">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="26b62-114">supportDeviceLicensing</span></span>|<span data-ttu-id="26b62-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="26b62-115">Boolean</span></span>|<span data-ttu-id="26b62-116">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26b62-116">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="26b62-117">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="26b62-117">supportsUserLicensing</span></span>|<span data-ttu-id="26b62-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b62-118">Boolean</span></span>|<span data-ttu-id="26b62-119">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="26b62-119">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="26b62-120">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="26b62-120">supportsDeviceLicensing</span></span>|<span data-ttu-id="26b62-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="26b62-121">Boolean</span></span>|<span data-ttu-id="26b62-122">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26b62-122">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26b62-123">Relações</span><span class="sxs-lookup"><span data-stu-id="26b62-123">Relationships</span></span>
<span data-ttu-id="26b62-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26b62-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26b62-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26b62-125">JSON Representation</span></span>
<span data-ttu-id="26b62-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26b62-126">Here is a JSON representation of the resource.</span></span>
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



