---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 660265882a0b40e365dc49b0642f078ac4df73ea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950393"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="64c46-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="64c46-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="64c46-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64c46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64c46-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64c46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64c46-106">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="64c46-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="64c46-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64c46-107">Properties</span></span>
|<span data-ttu-id="64c46-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64c46-108">Property</span></span>|<span data-ttu-id="64c46-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="64c46-109">Type</span></span>|<span data-ttu-id="64c46-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="64c46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64c46-111">iPad</span><span class="sxs-lookup"><span data-stu-id="64c46-111">iPad</span></span>|<span data-ttu-id="64c46-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="64c46-112">Boolean</span></span>|<span data-ttu-id="64c46-113">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="64c46-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="64c46-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="64c46-114">iPhoneAndIPod</span></span>|<span data-ttu-id="64c46-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="64c46-115">Boolean</span></span>|<span data-ttu-id="64c46-116">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="64c46-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64c46-117">Relações</span><span class="sxs-lookup"><span data-stu-id="64c46-117">Relationships</span></span>
<span data-ttu-id="64c46-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64c46-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64c46-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64c46-119">JSON Representation</span></span>
<span data-ttu-id="64c46-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64c46-120">Here is a JSON representation of the resource.</span></span>
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




