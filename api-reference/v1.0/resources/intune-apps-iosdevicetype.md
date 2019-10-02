---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a62cb711b70352d98650ae03945316de9ed2b5d2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356249"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="93851-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="93851-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="93851-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93851-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93851-105">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="93851-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="93851-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93851-106">Properties</span></span>
|<span data-ttu-id="93851-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93851-107">Property</span></span>|<span data-ttu-id="93851-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="93851-108">Type</span></span>|<span data-ttu-id="93851-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="93851-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93851-110">iPad</span><span class="sxs-lookup"><span data-stu-id="93851-110">iPad</span></span>|<span data-ttu-id="93851-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="93851-111">Boolean</span></span>|<span data-ttu-id="93851-112">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="93851-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="93851-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="93851-113">iPhoneAndIPod</span></span>|<span data-ttu-id="93851-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="93851-114">Boolean</span></span>|<span data-ttu-id="93851-115">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="93851-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93851-116">Relações</span><span class="sxs-lookup"><span data-stu-id="93851-116">Relationships</span></span>
<span data-ttu-id="93851-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93851-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93851-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93851-118">JSON Representation</span></span>
<span data-ttu-id="93851-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93851-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```




