---
title: Tipo de recurso do iosDeviceType
description: Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9751d541b0bcb64b68673aa8ca646fb85e70b5f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991300"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="6dbc3-103">Tipo de recurso do iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="6dbc3-103">iosDeviceType resource type</span></span>

> <span data-ttu-id="6dbc3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6dbc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dbc3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6dbc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dbc3-106">Contém propriedades de possíveis tipos de dispositivos de iOS que o aplicativo móvel pode executar.</span><span class="sxs-lookup"><span data-stu-id="6dbc3-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="6dbc3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6dbc3-107">Properties</span></span>
|<span data-ttu-id="6dbc3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dbc3-108">Property</span></span>|<span data-ttu-id="6dbc3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dbc3-109">Type</span></span>|<span data-ttu-id="6dbc3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dbc3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dbc3-111">iPad</span><span class="sxs-lookup"><span data-stu-id="6dbc3-111">iPad</span></span>|<span data-ttu-id="6dbc3-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="6dbc3-112">Boolean</span></span>|<span data-ttu-id="6dbc3-113">Se o aplicativo deve ser executado em iPads.</span><span class="sxs-lookup"><span data-stu-id="6dbc3-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="6dbc3-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="6dbc3-114">iPhoneAndIPod</span></span>|<span data-ttu-id="6dbc3-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="6dbc3-115">Boolean</span></span>|<span data-ttu-id="6dbc3-116">Se o aplicativo deve ser executado em iPhones e iPods.</span><span class="sxs-lookup"><span data-stu-id="6dbc3-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dbc3-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6dbc3-117">Relationships</span></span>
<span data-ttu-id="6dbc3-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6dbc3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6dbc3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6dbc3-119">JSON Representation</span></span>
<span data-ttu-id="6dbc3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6dbc3-120">Here is a JSON representation of the resource.</span></span>
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





