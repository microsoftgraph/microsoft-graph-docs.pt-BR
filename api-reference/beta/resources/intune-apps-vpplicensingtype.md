---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4b7983d20f22be5f8cce24a5c362926d00de55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851594"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="069c3-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="069c3-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="069c3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="069c3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="069c3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="069c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="069c3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="069c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="069c3-107">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="069c3-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="069c3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="069c3-108">Properties</span></span>
|<span data-ttu-id="069c3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="069c3-109">Property</span></span>|<span data-ttu-id="069c3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="069c3-110">Type</span></span>|<span data-ttu-id="069c3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="069c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="069c3-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="069c3-112">supportUserLicensing</span></span>|<span data-ttu-id="069c3-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="069c3-113">Boolean</span></span>|<span data-ttu-id="069c3-114">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="069c3-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="069c3-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="069c3-115">supportDeviceLicensing</span></span>|<span data-ttu-id="069c3-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="069c3-116">Boolean</span></span>|<span data-ttu-id="069c3-117">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="069c3-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="069c3-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="069c3-118">supportsUserLicensing</span></span>|<span data-ttu-id="069c3-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="069c3-119">Boolean</span></span>|<span data-ttu-id="069c3-120">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="069c3-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="069c3-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="069c3-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="069c3-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="069c3-122">Boolean</span></span>|<span data-ttu-id="069c3-123">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="069c3-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="069c3-124">Relações</span><span class="sxs-lookup"><span data-stu-id="069c3-124">Relationships</span></span>
<span data-ttu-id="069c3-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="069c3-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="069c3-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="069c3-126">JSON Representation</span></span>
<span data-ttu-id="069c3-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="069c3-127">Here is a JSON representation of the resource.</span></span>
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





