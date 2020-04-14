---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfe7f7e0340fbbe8c223694a172b1a77986863e6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459065"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="7f0e2-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="7f0e2-103">iosDeviceType resource type</span></span>

<span data-ttu-id="7f0e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f0e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f0e2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f0e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f0e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f0e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f0e2-107">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="7f0e2-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="7f0e2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f0e2-108">Properties</span></span>
|<span data-ttu-id="7f0e2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f0e2-109">Property</span></span>|<span data-ttu-id="7f0e2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f0e2-110">Type</span></span>|<span data-ttu-id="7f0e2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f0e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f0e2-112">iPad</span><span class="sxs-lookup"><span data-stu-id="7f0e2-112">iPad</span></span>|<span data-ttu-id="7f0e2-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="7f0e2-113">Boolean</span></span>|<span data-ttu-id="7f0e2-114">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="7f0e2-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="7f0e2-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="7f0e2-115">iPhoneAndIPod</span></span>|<span data-ttu-id="7f0e2-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="7f0e2-116">Boolean</span></span>|<span data-ttu-id="7f0e2-117">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="7f0e2-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f0e2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="7f0e2-118">Relationships</span></span>
<span data-ttu-id="7f0e2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f0e2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f0e2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f0e2-120">JSON Representation</span></span>
<span data-ttu-id="7f0e2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f0e2-121">Here is a JSON representation of the resource.</span></span>
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



