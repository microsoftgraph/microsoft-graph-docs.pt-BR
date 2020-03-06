---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 057de993f7e9cef948c3334b8dcb22e34f49ba23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531234"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="76838-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="76838-103">iosDeviceType resource type</span></span>

<span data-ttu-id="76838-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76838-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76838-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76838-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76838-106">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="76838-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="76838-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76838-107">Properties</span></span>
|<span data-ttu-id="76838-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76838-108">Property</span></span>|<span data-ttu-id="76838-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="76838-109">Type</span></span>|<span data-ttu-id="76838-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="76838-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76838-111">iPad</span><span class="sxs-lookup"><span data-stu-id="76838-111">iPad</span></span>|<span data-ttu-id="76838-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="76838-112">Boolean</span></span>|<span data-ttu-id="76838-113">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="76838-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="76838-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="76838-114">iPhoneAndIPod</span></span>|<span data-ttu-id="76838-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="76838-115">Boolean</span></span>|<span data-ttu-id="76838-116">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="76838-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76838-117">Relações</span><span class="sxs-lookup"><span data-stu-id="76838-117">Relationships</span></span>
<span data-ttu-id="76838-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76838-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76838-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76838-119">JSON Representation</span></span>
<span data-ttu-id="76838-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76838-120">Here is a JSON representation of the resource.</span></span>
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




