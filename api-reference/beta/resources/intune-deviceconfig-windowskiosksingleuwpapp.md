---
title: tipo de recurso windowsKioskSingleUWPApp
description: A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 804dd2f34416eecb956b322a0f178daaf39b2418
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142039"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="d203e-103">tipo de recurso windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="d203e-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="d203e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d203e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d203e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d203e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d203e-106">A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="d203e-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="d203e-107">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d203e-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d203e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d203e-108">Properties</span></span>
|<span data-ttu-id="d203e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d203e-109">Property</span></span>|<span data-ttu-id="d203e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d203e-110">Type</span></span>|<span data-ttu-id="d203e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d203e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d203e-112">uwpApp</span><span class="sxs-lookup"><span data-stu-id="d203e-112">uwpApp</span></span>|[<span data-ttu-id="d203e-113">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="d203e-113">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="d203e-114">Esta é a única ID de modelo de usuário do aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo quiosque</span><span class="sxs-lookup"><span data-stu-id="d203e-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="d203e-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d203e-115">Relationships</span></span>
<span data-ttu-id="d203e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d203e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d203e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d203e-117">JSON Representation</span></span>
<span data-ttu-id="d203e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d203e-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




