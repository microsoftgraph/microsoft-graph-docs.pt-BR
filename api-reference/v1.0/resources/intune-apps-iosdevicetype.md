---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b541310ced9c9aaa781077639203950d00f56f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976748"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="1aab7-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1aab7-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="1aab7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1aab7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1aab7-105">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="1aab7-105">Contains properties of the possible iOS device types the mobile app can run on.</span></span>
## <a name="properties"></a><span data-ttu-id="1aab7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1aab7-106">Properties</span></span>
|<span data-ttu-id="1aab7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1aab7-107">Property</span></span>|<span data-ttu-id="1aab7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aab7-108">Type</span></span>|<span data-ttu-id="1aab7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aab7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aab7-110">iPad</span><span class="sxs-lookup"><span data-stu-id="1aab7-110">iPad</span></span>|<span data-ttu-id="1aab7-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="1aab7-111">Boolean</span></span>|<span data-ttu-id="1aab7-112">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="1aab7-112">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="1aab7-113">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="1aab7-113">iPhoneAndIPod</span></span>|<span data-ttu-id="1aab7-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="1aab7-114">Boolean</span></span>|<span data-ttu-id="1aab7-115">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="1aab7-115">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aab7-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1aab7-116">Relationships</span></span>
<span data-ttu-id="1aab7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1aab7-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1aab7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1aab7-118">JSON Representation</span></span>
<span data-ttu-id="1aab7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1aab7-119">Here is a JSON representation of the resource.</span></span>
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



