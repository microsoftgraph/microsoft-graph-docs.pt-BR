---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 587c5e319490807369590585e53a06e0dcc7f2bb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37369055"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="f6f01-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="f6f01-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="f6f01-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6f01-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6f01-105">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="f6f01-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="f6f01-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6f01-106">Properties</span></span>
|<span data-ttu-id="f6f01-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6f01-107">Property</span></span>|<span data-ttu-id="f6f01-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6f01-108">Type</span></span>|<span data-ttu-id="f6f01-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6f01-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6f01-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="f6f01-110">supportsUserLicensing</span></span>|<span data-ttu-id="f6f01-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6f01-111">Boolean</span></span>|<span data-ttu-id="f6f01-112">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="f6f01-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="f6f01-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="f6f01-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="f6f01-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6f01-114">Boolean</span></span>|<span data-ttu-id="f6f01-115">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f6f01-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6f01-116">Relações</span><span class="sxs-lookup"><span data-stu-id="f6f01-116">Relationships</span></span>
<span data-ttu-id="f6f01-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6f01-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6f01-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6f01-118">JSON Representation</span></span>
<span data-ttu-id="f6f01-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6f01-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```




