---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f31388de57835ea91ae3dc9fd104dd3b74b0ae32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43362762"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="c3e4e-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="c3e4e-103">vppLicensingType resource type</span></span>

<span data-ttu-id="c3e4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3e4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3e4e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c3e4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3e4e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3e4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3e4e-107">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="c3e4e-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="c3e4e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3e4e-108">Properties</span></span>
|<span data-ttu-id="c3e4e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3e4e-109">Property</span></span>|<span data-ttu-id="c3e4e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3e4e-110">Type</span></span>|<span data-ttu-id="c3e4e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3e4e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3e4e-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="c3e4e-112">supportUserLicensing</span></span>|<span data-ttu-id="c3e4e-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3e4e-113">Boolean</span></span>|<span data-ttu-id="c3e4e-114">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3e4e-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="c3e4e-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="c3e4e-115">supportDeviceLicensing</span></span>|<span data-ttu-id="c3e4e-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3e4e-116">Boolean</span></span>|<span data-ttu-id="c3e4e-117">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3e4e-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="c3e4e-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="c3e4e-118">supportsUserLicensing</span></span>|<span data-ttu-id="c3e4e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3e4e-119">Boolean</span></span>|<span data-ttu-id="c3e4e-120">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="c3e4e-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="c3e4e-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="c3e4e-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="c3e4e-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3e4e-122">Boolean</span></span>|<span data-ttu-id="c3e4e-123">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c3e4e-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3e4e-124">Relações</span><span class="sxs-lookup"><span data-stu-id="c3e4e-124">Relationships</span></span>
<span data-ttu-id="c3e4e-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3e4e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3e4e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3e4e-126">JSON Representation</span></span>
<span data-ttu-id="c3e4e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3e4e-127">Here is a JSON representation of the resource.</span></span>
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



