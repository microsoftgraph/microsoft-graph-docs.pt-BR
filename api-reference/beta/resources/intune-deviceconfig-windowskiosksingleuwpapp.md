---
title: tipo de recurso de windowsKioskSingleUWPApp
description: A classe usada para identificar as informações de app UWP para a configuração de quiosque
author: tfitzmac
ms.openlocfilehash: fd1dffd5a01b89db27132770d4c8ffe0094eed8f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312177"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a><span data-ttu-id="2c3a0-103">tipo de recurso de windowsKioskSingleUWPApp</span><span class="sxs-lookup"><span data-stu-id="2c3a0-103">windowsKioskSingleUWPApp resource type</span></span>

> <span data-ttu-id="2c3a0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2c3a0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c3a0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2c3a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c3a0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2c3a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c3a0-107">A classe usada para identificar as informações de app UWP para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="2c3a0-107">The class used to identify the UWP app info for the kiosk configuration</span></span>

<span data-ttu-id="2c3a0-108">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c3a0-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c3a0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c3a0-109">Properties</span></span>
|<span data-ttu-id="2c3a0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c3a0-110">Property</span></span>|<span data-ttu-id="2c3a0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c3a0-111">Type</span></span>|<span data-ttu-id="2c3a0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c3a0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c3a0-113">uwpApp</span><span class="sxs-lookup"><span data-stu-id="2c3a0-113">uwpApp</span></span>|[<span data-ttu-id="2c3a0-114">windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="2c3a0-114">windowsKioskUWPApp</span></span>](../resources/intune-deviceconfig-windowskioskuwpapp.md)|<span data-ttu-id="2c3a0-115">Este é o único aplicativo usuário modelo ID (AUMID) que estarão disponíveis para uso no modo de quiosque de início</span><span class="sxs-lookup"><span data-stu-id="2c3a0-115">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c3a0-116">Relações</span><span class="sxs-lookup"><span data-stu-id="2c3a0-116">Relationships</span></span>
<span data-ttu-id="2c3a0-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c3a0-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c3a0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c3a0-118">JSON Representation</span></span>
<span data-ttu-id="2c3a0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c3a0-119">Here is a JSON representation of the resource.</span></span>
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
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```





