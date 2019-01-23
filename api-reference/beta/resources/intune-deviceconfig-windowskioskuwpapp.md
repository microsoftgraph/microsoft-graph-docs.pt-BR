---
title: tipo de recurso de windowsKioskUWPApp
description: A classe base para um tipo de aplicativos
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ba5367721890f02af3b348ad469b15024de4800
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392679"
---
# <a name="windowskioskuwpapp-resource-type"></a><span data-ttu-id="46c03-103">tipo de recurso de windowsKioskUWPApp</span><span class="sxs-lookup"><span data-stu-id="46c03-103">windowsKioskUWPApp resource type</span></span>

> <span data-ttu-id="46c03-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="46c03-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46c03-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46c03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46c03-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="46c03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46c03-107">A classe base para um tipo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="46c03-107">The base class for a type of apps</span></span>


<span data-ttu-id="46c03-108">Herda de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="46c03-108">Inherits from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46c03-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46c03-109">Properties</span></span>
|<span data-ttu-id="46c03-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46c03-110">Property</span></span>|<span data-ttu-id="46c03-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="46c03-111">Type</span></span>|<span data-ttu-id="46c03-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="46c03-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46c03-113">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="46c03-113">startLayoutTileSize</span></span>|[<span data-ttu-id="46c03-114">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="46c03-114">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="46c03-115">O tamanho de blocos de aplicativo para o layout de iniciar Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="46c03-115">The app tile size for the start layout Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="46c03-116">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="46c03-116">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="46c03-117">name</span><span class="sxs-lookup"><span data-stu-id="46c03-117">name</span></span>|<span data-ttu-id="46c03-118">String</span><span class="sxs-lookup"><span data-stu-id="46c03-118">String</span></span>|<span data-ttu-id="46c03-119">Representa o nome amigável de um aplicativo Inherited de [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="46c03-119">Represents the friendly name of an app Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span></span>|
|<span data-ttu-id="46c03-120">tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="46c03-120">appType</span></span>|[<span data-ttu-id="46c03-121">windowsKioskAppType</span><span class="sxs-lookup"><span data-stu-id="46c03-121">windowsKioskAppType</span></span>](../resources/intune-deviceconfig-windowskioskapptype.md)|<span data-ttu-id="46c03-122">O tipo de app Inherited da [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span><span class="sxs-lookup"><span data-stu-id="46c03-122">The app type Inherited from [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md).</span></span> <span data-ttu-id="46c03-123">Os valores possíveis são: `unknown`, `store`, `desktop`, `aumId`.</span><span class="sxs-lookup"><span data-stu-id="46c03-123">Possible values are: `unknown`, `store`, `desktop`, `aumId`.</span></span>|
|<span data-ttu-id="46c03-124">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="46c03-124">appUserModelId</span></span>|<span data-ttu-id="46c03-125">String</span><span class="sxs-lookup"><span data-stu-id="46c03-125">String</span></span>|<span data-ttu-id="46c03-126">Este é o único aplicativo usuário modelo ID (AUMID) que estarão disponíveis para uso no modo de quiosque de início</span><span class="sxs-lookup"><span data-stu-id="46c03-126">This is the only Application User Model ID (AUMID) that will be available to launch use while in Kiosk Mode</span></span>|
|<span data-ttu-id="46c03-127">appId</span><span class="sxs-lookup"><span data-stu-id="46c03-127">appId</span></span>|<span data-ttu-id="46c03-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46c03-128">String</span></span>|<span data-ttu-id="46c03-129">Isso faz referência a um App Intune que será o destino para as atribuições mesmos como a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="46c03-129">This references an Intune App that will be target to the same assignments as Kiosk configuration</span></span>|
|<span data-ttu-id="46c03-130">containedAppId</span><span class="sxs-lookup"><span data-stu-id="46c03-130">containedAppId</span></span>|<span data-ttu-id="46c03-131">String</span><span class="sxs-lookup"><span data-stu-id="46c03-131">String</span></span>|<span data-ttu-id="46c03-132">Isso faz referência a um aplicativo contido de um App Intune</span><span class="sxs-lookup"><span data-stu-id="46c03-132">This references an contained App from an Intune App</span></span>|

## <a name="relationships"></a><span data-ttu-id="46c03-133">Relações</span><span class="sxs-lookup"><span data-stu-id="46c03-133">Relationships</span></span>
<span data-ttu-id="46c03-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46c03-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46c03-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46c03-135">JSON Representation</span></span>
<span data-ttu-id="46c03-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46c03-136">Here is a JSON representation of the resource.</span></span>
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
  "appType": "String",
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




