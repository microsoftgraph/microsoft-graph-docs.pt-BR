---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c842d27d3113210d96479388d2395b24dea8f123
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798123"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="43893-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="43893-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="43893-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="43893-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43893-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43893-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43893-106">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="43893-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="43893-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43893-107">Properties</span></span>
|<span data-ttu-id="43893-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43893-108">Property</span></span>|<span data-ttu-id="43893-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="43893-109">Type</span></span>|<span data-ttu-id="43893-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="43893-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43893-111">iPad</span><span class="sxs-lookup"><span data-stu-id="43893-111">iPad</span></span>|<span data-ttu-id="43893-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="43893-112">Boolean</span></span>|<span data-ttu-id="43893-113">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="43893-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="43893-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="43893-114">iPhoneAndIPod</span></span>|<span data-ttu-id="43893-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="43893-115">Boolean</span></span>|<span data-ttu-id="43893-116">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="43893-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43893-117">Relações</span><span class="sxs-lookup"><span data-stu-id="43893-117">Relationships</span></span>
<span data-ttu-id="43893-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43893-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43893-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43893-119">JSON Representation</span></span>
<span data-ttu-id="43893-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43893-120">Here is a JSON representation of the resource.</span></span>
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



