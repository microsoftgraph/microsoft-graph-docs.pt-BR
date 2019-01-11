---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ffa46d1e8fb693822051250fb4a722815b1dcb73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866777"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="02c60-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="02c60-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="02c60-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="02c60-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02c60-105">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="02c60-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="02c60-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02c60-106">Properties</span></span>
|<span data-ttu-id="02c60-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02c60-107">Property</span></span>|<span data-ttu-id="02c60-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="02c60-108">Type</span></span>|<span data-ttu-id="02c60-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="02c60-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02c60-110">iPad</span><span class="sxs-lookup"><span data-stu-id="02c60-110">iPad</span></span>|<span data-ttu-id="02c60-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="02c60-111">Boolean</span></span>|<span data-ttu-id="02c60-112">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="02c60-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="02c60-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="02c60-113">iPhoneAndIPod</span></span>|<span data-ttu-id="02c60-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="02c60-114">Boolean</span></span>|<span data-ttu-id="02c60-115">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="02c60-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02c60-116">Relações</span><span class="sxs-lookup"><span data-stu-id="02c60-116">Relationships</span></span>
<span data-ttu-id="02c60-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="02c60-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="02c60-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02c60-118">JSON Representation</span></span>
<span data-ttu-id="02c60-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02c60-119">Here is a JSON representation of the resource.</span></span>
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



