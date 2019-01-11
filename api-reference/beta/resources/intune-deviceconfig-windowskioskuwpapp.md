---
title: tipo de recurso de windowsKioskUWPApp
description: A classe base para um tipo de aplicativos
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8f456841962b399a1e9687017a0a8eaeb07a4ba7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871859"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="af2a1-103">tipo de recurso de windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="af2a1-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="af2a1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="af2a1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af2a1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af2a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af2a1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="af2a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af2a1-107">A classe base para um tipo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="af2a1-107">The base class for a type of apps</span></span>

<span data-ttu-id="af2a1-108">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="af2a1-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af2a1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af2a1-109">Properties</span></span>
|<span data-ttu-id="af2a1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af2a1-110">Property</span></span>|<span data-ttu-id="af2a1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="af2a1-111">Type</span></span>|<span data-ttu-id="af2a1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="af2a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af2a1-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="af2a1-113">startLayoutTileSize</span></span>|[<span data-ttu-id="af2a1-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="af2a1-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="af2a1-115">O tamanho de blocos de aplicativo para o layout de iniciar Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="af2a1-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="af2a1-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="af2a1-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="af2a1-117">name</span><span class="sxs-lookup"><span data-stu-id="af2a1-117">name</span></span>|<span data-ttu-id="af2a1-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af2a1-118">String</span></span>|<span data-ttu-id="af2a1-119">Representa o nome amigável de um aplicativo Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="af2a1-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="af2a1-120">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="af2a1-120">appUserModelId</span></span>|<span data-ttu-id="af2a1-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af2a1-121">String</span></span>|<span data-ttu-id="af2a1-122">Este é o único aplicativo usuário modelo ID (AUMID) que estarão disponíveis para uso no modo de quiosque de início</span><span class="sxs-lookup"><span data-stu-id="af2a1-122">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="af2a1-123">appId</span><span class="sxs-lookup"><span data-stu-id="af2a1-123">appId</span></span>|<span data-ttu-id="af2a1-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af2a1-124">String</span></span>|<span data-ttu-id="af2a1-125">Isso faz referência a um App Intune que será o destino para as atribuições mesmos como a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="af2a1-125">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="af2a1-126">containedAppId</span><span class="sxs-lookup"><span data-stu-id="af2a1-126">containedAppId</span></span>|<span data-ttu-id="af2a1-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af2a1-127">String</span></span>|<span data-ttu-id="af2a1-128">Isso faz referência a um aplicativo contido de um App Intune</span><span class="sxs-lookup"><span data-stu-id="af2a1-128">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="af2a1-129">Relações</span><span class="sxs-lookup"><span data-stu-id="af2a1-129">Relationships</span></span>
<span data-ttu-id="af2a1-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af2a1-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="af2a1-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af2a1-131">JSON Representation</span></span>
<span data-ttu-id="af2a1-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af2a1-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





