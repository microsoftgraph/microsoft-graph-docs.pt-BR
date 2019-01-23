---
title: Tipo de recurso vppLicensingType
description: Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42bb678077781309b9e06c339112537bc2e48bde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399672"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="889d4-103">Tipo de recurso vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="889d4-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="889d4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="889d4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="889d4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="889d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="889d4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="889d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="889d4-107">Contém propriedades para o tipo de licenciamento iOS Volume-Purchased Program (VPP).</span><span class="sxs-lookup"><span data-stu-id="889d4-107">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="889d4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="889d4-108">Properties</span></span>
|<span data-ttu-id="889d4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="889d4-109">Property</span></span>|<span data-ttu-id="889d4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="889d4-110">Type</span></span>|<span data-ttu-id="889d4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="889d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="889d4-112">supportUserLicensing</span><span class="sxs-lookup"><span data-stu-id="889d4-112">supportUserLicensing</span></span>|<span data-ttu-id="889d4-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="889d4-113">Boolean</span></span>|<span data-ttu-id="889d4-114">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="889d4-114">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="889d4-115">supportDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="889d4-115">supportDeviceLicensing</span></span>|<span data-ttu-id="889d4-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="889d4-116">Boolean</span></span>|<span data-ttu-id="889d4-117">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="889d4-117">Whether the program supports the device licensing type.</span></span>|
|<span data-ttu-id="889d4-118">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="889d4-118">supportsUserLicensing</span></span>|<span data-ttu-id="889d4-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="889d4-119">Boolean</span></span>|<span data-ttu-id="889d4-120">Se o programa dá suporte ao tipo de licença do usuário.</span><span class="sxs-lookup"><span data-stu-id="889d4-120">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="889d4-121">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="889d4-121">supportsDeviceLicensing</span></span>|<span data-ttu-id="889d4-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="889d4-122">Boolean</span></span>|<span data-ttu-id="889d4-123">Se o programa dá suporte ao tipo de licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="889d4-123">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="889d4-124">Relações</span><span class="sxs-lookup"><span data-stu-id="889d4-124">Relationships</span></span>
<span data-ttu-id="889d4-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="889d4-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="889d4-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="889d4-126">JSON Representation</span></span>
<span data-ttu-id="889d4-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="889d4-127">Here is a JSON representation of the resource.</span></span>
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




