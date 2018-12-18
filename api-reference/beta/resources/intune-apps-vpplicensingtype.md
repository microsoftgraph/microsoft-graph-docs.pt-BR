---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: tfitzmac
ms.openlocfilehash: 83e68cc018b3e3f5948b105118bffbeb93010c2f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351300"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="20ae6-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="20ae6-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="20ae6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="20ae6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20ae6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="20ae6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20ae6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="20ae6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20ae6-107">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="20ae6-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="20ae6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20ae6-108">Properties</span></span>
|<span data-ttu-id="20ae6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20ae6-109">Property</span></span>|<span data-ttu-id="20ae6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="20ae6-110">Type</span></span>|<span data-ttu-id="20ae6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="20ae6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20ae6-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="20ae6-112">supportUserLicensing</span></span>|<span data-ttu-id="20ae6-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="20ae6-113">Boolean</span></span>|<span data-ttu-id="20ae6-114">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="20ae6-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="20ae6-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="20ae6-115">supportDeviceLicensing</span></span>|<span data-ttu-id="20ae6-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="20ae6-116">Boolean</span></span>|<span data-ttu-id="20ae6-117">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20ae6-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="20ae6-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="20ae6-118">supportsUserLicensing</span></span>|<span data-ttu-id="20ae6-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="20ae6-119">Boolean</span></span>|<span data-ttu-id="20ae6-120">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="20ae6-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="20ae6-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="20ae6-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="20ae6-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="20ae6-122">Boolean</span></span>|<span data-ttu-id="20ae6-123">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20ae6-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20ae6-124">Relações</span><span class="sxs-lookup"><span data-stu-id="20ae6-124">Relationships</span></span>
<span data-ttu-id="20ae6-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20ae6-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20ae6-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20ae6-126">JSON Representation</span></span>
<span data-ttu-id="20ae6-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20ae6-127">Here is a JSON representation of the resource.</span></span>
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





