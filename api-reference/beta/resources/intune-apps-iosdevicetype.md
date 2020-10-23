---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19dc8db9f4d5a619add49e6693b97d8175c5e6da
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730767"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="d4a1a-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d4a1a-103">iosDeviceType resource type</span></span>

<span data-ttu-id="d4a1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4a1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4a1a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4a1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4a1a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4a1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4a1a-107">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="d4a1a-107">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="d4a1a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4a1a-108">Properties</span></span>
|<span data-ttu-id="d4a1a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4a1a-109">Property</span></span>|<span data-ttu-id="d4a1a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4a1a-110">Type</span></span>|<span data-ttu-id="d4a1a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4a1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4a1a-112">iPad</span><span class="sxs-lookup"><span data-stu-id="d4a1a-112">iPad</span></span>|<span data-ttu-id="d4a1a-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4a1a-113">Boolean</span></span>|<span data-ttu-id="d4a1a-114">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="d4a1a-114">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="d4a1a-115">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="d4a1a-115">iPhoneAndIPod</span></span>|<span data-ttu-id="d4a1a-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4a1a-116">Boolean</span></span>|<span data-ttu-id="d4a1a-117">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="d4a1a-117">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4a1a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="d4a1a-118">Relationships</span></span>
<span data-ttu-id="d4a1a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4a1a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4a1a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4a1a-120">JSON Representation</span></span>
<span data-ttu-id="d4a1a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4a1a-121">Here is a JSON representation of the resource.</span></span>
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





