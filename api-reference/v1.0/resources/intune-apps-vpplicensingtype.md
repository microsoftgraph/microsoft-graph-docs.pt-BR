---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: tfitzmac
ms.openlocfilehash: 7958266fe208e0a04bc72ab658291c58455c763b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322558"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="56a8e-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="56a8e-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="56a8e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="56a8e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56a8e-105">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="56a8e-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="56a8e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56a8e-106">Properties</span></span>
|<span data-ttu-id="56a8e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56a8e-107">Property</span></span>|<span data-ttu-id="56a8e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="56a8e-108">Type</span></span>|<span data-ttu-id="56a8e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="56a8e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56a8e-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="56a8e-110">supportsUserLicensing</span></span>|<span data-ttu-id="56a8e-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="56a8e-111">Boolean</span></span>|<span data-ttu-id="56a8e-112">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="56a8e-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="56a8e-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="56a8e-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="56a8e-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="56a8e-114">Boolean</span></span>|<span data-ttu-id="56a8e-115">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56a8e-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56a8e-116">Relações</span><span class="sxs-lookup"><span data-stu-id="56a8e-116">Relationships</span></span>
<span data-ttu-id="56a8e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56a8e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56a8e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56a8e-118">JSON Representation</span></span>
<span data-ttu-id="56a8e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56a8e-119">Here is a JSON representation of the resource.</span></span>
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



