---
title: Tipo de recurso windowsKioskSingleWin32App
description: A classe usada para identificar a configuração de aplicativo único para a configuração do quiosque win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fefde9fa13849a910c56e4ebaed870ebb9edac62
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446193"
---
# <a name="windowskiosksinglewin32app-resource-type"></a><span data-ttu-id="e3a32-103">Tipo de recurso windowsKioskSingleWin32App</span><span class="sxs-lookup"><span data-stu-id="e3a32-103">windowsKioskSingleWin32App resource type</span></span>

<span data-ttu-id="e3a32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3a32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3a32-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3a32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3a32-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3a32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3a32-107">A classe usada para identificar a configuração de aplicativo único para a configuração do quiosque win32</span><span class="sxs-lookup"><span data-stu-id="e3a32-107">The class used to identify the single app configuration for the kiosk win32 configuration</span></span>


<span data-ttu-id="e3a32-108">Herda do [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3a32-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3a32-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3a32-109">Properties</span></span>
|<span data-ttu-id="e3a32-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3a32-110">Property</span></span>|<span data-ttu-id="e3a32-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3a32-111">Type</span></span>|<span data-ttu-id="e3a32-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3a32-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3a32-113">win32App</span><span class="sxs-lookup"><span data-stu-id="e3a32-113">win32App</span></span>|[<span data-ttu-id="e3a32-114">windowsKioskWin32App</span><span class="sxs-lookup"><span data-stu-id="e3a32-114">windowsKioskWin32App</span></span>](../resources/intune-deviceconfig-windowskioskwin32app.md)|<span data-ttu-id="e3a32-115">Este é o aplicativo win32 que estará disponível para iniciar o uso enquanto estiver no modo Quiosque</span><span class="sxs-lookup"><span data-stu-id="e3a32-115">This is the win32 app that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3a32-116">Relações</span><span class="sxs-lookup"><span data-stu-id="e3a32-116">Relationships</span></span>
<span data-ttu-id="e3a32-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3a32-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3a32-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3a32-118">JSON Representation</span></span>
<span data-ttu-id="e3a32-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3a32-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleWin32App",
  "win32App": {
    "@odata.type": "microsoft.graph.windowsKioskWin32App",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "classicAppPath": "String",
    "edgeNoFirstRun": true,
    "edgeKioskIdleTimeoutMinutes": 1024,
    "edgeKioskType": "String",
    "edgeKiosk": "String"
  }
}
```




