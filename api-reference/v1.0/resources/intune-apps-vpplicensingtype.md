---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df7d130b1ee3354a0a82788ce58543b9eb6e7896
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439642"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="3805a-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="3805a-103">vppLicensingType resource type</span></span>

<span data-ttu-id="3805a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3805a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3805a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3805a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3805a-106">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="3805a-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="3805a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3805a-107">Properties</span></span>
|<span data-ttu-id="3805a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3805a-108">Property</span></span>|<span data-ttu-id="3805a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3805a-109">Type</span></span>|<span data-ttu-id="3805a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3805a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3805a-111">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="3805a-111">supportsUserLicensing</span></span>|<span data-ttu-id="3805a-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="3805a-112">Boolean</span></span>|<span data-ttu-id="3805a-113">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="3805a-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="3805a-114">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="3805a-114">supportsDeviceLicensing</span></span>|<span data-ttu-id="3805a-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="3805a-115">Boolean</span></span>|<span data-ttu-id="3805a-116">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3805a-116">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3805a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="3805a-117">Relationships</span></span>
<span data-ttu-id="3805a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3805a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3805a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3805a-119">JSON Representation</span></span>
<span data-ttu-id="3805a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3805a-120">Here is a JSON representation of the resource.</span></span>
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







