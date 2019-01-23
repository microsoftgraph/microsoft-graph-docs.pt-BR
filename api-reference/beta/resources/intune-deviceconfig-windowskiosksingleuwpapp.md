---
title: tipo de recurso de windowsKioskSingleUWPApp
description: A classe usada para identificar as informações de app UWP para a configuração de quiosque
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e62dc6393cc2dc6a9133732a42527abdfadbd91e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409374"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="cc884-103">tipo de recurso de windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="cc884-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="cc884-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cc884-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc884-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cc884-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc884-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cc884-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc884-107">A classe usada para identificar as informações de app UWP para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="cc884-107">The class used to identify the UWP app info for the kiosk configuration</span></span>


<span data-ttu-id="cc884-108">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc884-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cc884-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc884-109">Properties</span></span>
|<span data-ttu-id="cc884-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc884-110">Property</span></span>|<span data-ttu-id="cc884-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc884-111">Type</span></span>|<span data-ttu-id="cc884-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc884-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc884-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="cc884-113">uwpApp</span></span>|[<span data-ttu-id="cc884-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="cc884-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="cc884-115">Este é o único aplicativo usuário modelo ID (AUMID) que estarão disponíveis para uso no modo de quiosque de início</span><span class="sxs-lookup"><span data-stu-id="cc884-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc884-116">Relações</span><span class="sxs-lookup"><span data-stu-id="cc884-116">Relationships</span></span>
<span data-ttu-id="cc884-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc884-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc884-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc884-118">JSON Representation</span></span>
<span data-ttu-id="cc884-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc884-119">Here is a JSON representation of the resource.</span></span>
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




