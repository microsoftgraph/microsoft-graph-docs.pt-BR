---
title: tipo de recurso windowsKioskSingleUWPApp
description: A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 276cbe4c231425540037dcc9a9e0afe977220bc0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944009"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="5489a-103">tipo de recurso windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="5489a-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="5489a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5489a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5489a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5489a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5489a-106">A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="5489a-106">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="5489a-107">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5489a-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5489a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5489a-108">Properties</span></span>
|<span data-ttu-id="5489a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5489a-109">Property</span></span>|<span data-ttu-id="5489a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5489a-110">Type</span></span>|<span data-ttu-id="5489a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5489a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5489a-112">uwpApp</span><span class="sxs-lookup"><span data-stu-id="5489a-112">uwpApp</span></span>|[<span data-ttu-id="5489a-113">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="5489a-113">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="5489a-114">Esta é a única ID de modelo de usuário do aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo quiosque</span><span class="sxs-lookup"><span data-stu-id="5489a-114">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="5489a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="5489a-115">Relationships</span></span>
<span data-ttu-id="5489a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5489a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5489a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5489a-117">JSON Representation</span></span>
<span data-ttu-id="5489a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5489a-118">Here is a JSON representation of the resource.</span></span>
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
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```




