---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d142bf23686195d8e477901341af6ebdd03136b3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003917"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="3d62e-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3d62e-103">iosDeviceType resource type</span></span>

<span data-ttu-id="3d62e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d62e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d62e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d62e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d62e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d62e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d62e-107">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="3d62e-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="3d62e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d62e-108">Properties</span></span>
|<span data-ttu-id="3d62e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d62e-109">Property</span></span>|<span data-ttu-id="3d62e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d62e-110">Type</span></span>|<span data-ttu-id="3d62e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d62e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d62e-112">iPad</span><span class="sxs-lookup"><span data-stu-id="3d62e-112">iPad</span></span>|<span data-ttu-id="3d62e-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="3d62e-113">Boolean</span></span>|<span data-ttu-id="3d62e-114">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="3d62e-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="3d62e-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="3d62e-115">iPhoneAndIPod</span></span>|<span data-ttu-id="3d62e-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="3d62e-116">Boolean</span></span>|<span data-ttu-id="3d62e-117">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="3d62e-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d62e-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3d62e-118">Relationships</span></span>
<span data-ttu-id="3d62e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d62e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d62e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d62e-120">JSON Representation</span></span>
<span data-ttu-id="3d62e-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d62e-121">Here is a JSON representation of the resource.</span></span>
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






