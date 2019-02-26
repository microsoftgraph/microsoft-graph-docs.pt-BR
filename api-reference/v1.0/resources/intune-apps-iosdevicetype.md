---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f3bd1d0aff7e09d5828496de348805075d0b330
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259742"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="08008-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="08008-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="08008-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08008-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08008-105">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="08008-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="08008-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08008-106">Properties</span></span>
|<span data-ttu-id="08008-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08008-107">Property</span></span>|<span data-ttu-id="08008-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="08008-108">Type</span></span>|<span data-ttu-id="08008-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="08008-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08008-110">iPad</span><span class="sxs-lookup"><span data-stu-id="08008-110">iPad</span></span>|<span data-ttu-id="08008-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="08008-111">Boolean</span></span>|<span data-ttu-id="08008-112">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="08008-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="08008-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="08008-113">iPhoneAndIPod</span></span>|<span data-ttu-id="08008-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="08008-114">Boolean</span></span>|<span data-ttu-id="08008-115">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="08008-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08008-116">Relações</span><span class="sxs-lookup"><span data-stu-id="08008-116">Relationships</span></span>
<span data-ttu-id="08008-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08008-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08008-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08008-118">JSON Representation</span></span>
<span data-ttu-id="08008-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08008-119">Here is a JSON representation of the resource.</span></span>
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



