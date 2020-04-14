---
title: tipo de recurso windowsKioskSingleUWPApp
description: A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 168317587a7e20fabd3754a96c3b65ebefef963c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464063"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="b7177-103">tipo de recurso windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="b7177-103">windowsKioskSingleUWPApp resource type</span></span>

<span data-ttu-id="b7177-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7177-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7177-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7177-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7177-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7177-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7177-107">A classe usada para identificar as informações do aplicativo UWP para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="b7177-107">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="b7177-108">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7177-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b7177-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7177-109">Properties</span></span>
|<span data-ttu-id="b7177-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7177-110">Property</span></span>|<span data-ttu-id="b7177-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7177-111">Type</span></span>|<span data-ttu-id="b7177-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7177-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7177-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="b7177-113">uwpApp</span></span>|[<span data-ttu-id="b7177-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="b7177-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="b7177-115">Esta é a única ID de modelo de usuário do aplicativo (AUMID) que estará disponível para iniciar o uso enquanto estiver no modo quiosque</span><span class="sxs-lookup"><span data-stu-id="b7177-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7177-116">Relações</span><span class="sxs-lookup"><span data-stu-id="b7177-116">Relationships</span></span>
<span data-ttu-id="b7177-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7177-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7177-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7177-118">JSON Representation</span></span>
<span data-ttu-id="b7177-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7177-119">Here is a JSON representation of the resource.</span></span>
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



