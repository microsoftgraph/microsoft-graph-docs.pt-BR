---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b46c9bcd8680ffbd78c1cfc85cc6dec85126e6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256116"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="d8c39-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="d8c39-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="d8c39-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8c39-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8c39-105">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="d8c39-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="d8c39-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8c39-106">Properties</span></span>
|<span data-ttu-id="d8c39-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8c39-107">Property</span></span>|<span data-ttu-id="d8c39-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8c39-108">Type</span></span>|<span data-ttu-id="d8c39-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8c39-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8c39-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="d8c39-110">supportsUserLicensing</span></span>|<span data-ttu-id="d8c39-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8c39-111">Boolean</span></span>|<span data-ttu-id="d8c39-112">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8c39-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="d8c39-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="d8c39-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="d8c39-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8c39-114">Boolean</span></span>|<span data-ttu-id="d8c39-115">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8c39-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8c39-116">Relações</span><span class="sxs-lookup"><span data-stu-id="d8c39-116">Relationships</span></span>
<span data-ttu-id="d8c39-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8c39-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8c39-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8c39-118">JSON Representation</span></span>
<span data-ttu-id="d8c39-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8c39-119">Here is a JSON representation of the resource.</span></span>
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



