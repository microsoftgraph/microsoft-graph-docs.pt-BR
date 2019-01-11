---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bbc52cfd4e14b2010dd133e4fa08e61a30fb63df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814109"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="8b405-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="8b405-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="8b405-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8b405-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b405-105">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="8b405-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="8b405-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b405-106">Properties</span></span>
|<span data-ttu-id="8b405-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b405-107">Property</span></span>|<span data-ttu-id="8b405-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b405-108">Type</span></span>|<span data-ttu-id="8b405-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b405-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b405-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="8b405-110">supportsUserLicensing</span></span>|<span data-ttu-id="8b405-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="8b405-111">Boolean</span></span>|<span data-ttu-id="8b405-112">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="8b405-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="8b405-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8b405-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="8b405-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="8b405-114">Boolean</span></span>|<span data-ttu-id="8b405-115">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8b405-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b405-116">Relações</span><span class="sxs-lookup"><span data-stu-id="8b405-116">Relationships</span></span>
<span data-ttu-id="8b405-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b405-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8b405-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b405-118">JSON Representation</span></span>
<span data-ttu-id="8b405-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b405-119">Here is a JSON representation of the resource.</span></span>
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



