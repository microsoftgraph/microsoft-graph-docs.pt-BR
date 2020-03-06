---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 72fc5365ee41bd281d4dd59ac81305066919752a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532746"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="254dd-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="254dd-103">vppLicensingType resource type</span></span>

<span data-ttu-id="254dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="254dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="254dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="254dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="254dd-106">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="254dd-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="254dd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="254dd-107">Properties</span></span>
|<span data-ttu-id="254dd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="254dd-108">Property</span></span>|<span data-ttu-id="254dd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="254dd-109">Type</span></span>|<span data-ttu-id="254dd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="254dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="254dd-111">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="254dd-111">supportsUserLicensing</span></span>|<span data-ttu-id="254dd-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="254dd-112">Boolean</span></span>|<span data-ttu-id="254dd-113">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="254dd-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="254dd-114">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="254dd-114">supportsDeviceLicensing</span></span>|<span data-ttu-id="254dd-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="254dd-115">Boolean</span></span>|<span data-ttu-id="254dd-116">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="254dd-116">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="254dd-117">Relações</span><span class="sxs-lookup"><span data-stu-id="254dd-117">Relationships</span></span>
<span data-ttu-id="254dd-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="254dd-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="254dd-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="254dd-119">JSON Representation</span></span>
<span data-ttu-id="254dd-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="254dd-120">Here is a JSON representation of the resource.</span></span>
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




