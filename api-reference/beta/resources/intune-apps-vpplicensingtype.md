---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 21d19579ef55b74280b7d2ddb3acb445aa18b864
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199998"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="e2886-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="e2886-103">vppLicensingType resource type</span></span>

<span data-ttu-id="e2886-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2886-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2886-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2886-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2886-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2886-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2886-107">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="e2886-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="e2886-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2886-108">Properties</span></span>
|<span data-ttu-id="e2886-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2886-109">Property</span></span>|<span data-ttu-id="e2886-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2886-110">Type</span></span>|<span data-ttu-id="e2886-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2886-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2886-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="e2886-112">supportUserLicensing</span></span>|<span data-ttu-id="e2886-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2886-113">Boolean</span></span>|<span data-ttu-id="e2886-114">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="e2886-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="e2886-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e2886-115">supportDeviceLicensing</span></span>|<span data-ttu-id="e2886-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2886-116">Boolean</span></span>|<span data-ttu-id="e2886-117">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2886-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="e2886-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="e2886-118">supportsUserLicensing</span></span>|<span data-ttu-id="e2886-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2886-119">Boolean</span></span>|<span data-ttu-id="e2886-120">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="e2886-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="e2886-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e2886-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="e2886-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2886-122">Boolean</span></span>|<span data-ttu-id="e2886-123">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2886-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2886-124">Relações</span><span class="sxs-lookup"><span data-stu-id="e2886-124">Relationships</span></span>
<span data-ttu-id="e2886-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2886-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2886-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2886-126">JSON Representation</span></span>
<span data-ttu-id="e2886-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2886-127">Here is a JSON representation of the resource.</span></span>
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




