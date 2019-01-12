---
title: tipo de recurso de windowsKioskMultipleApps
description: A classe usada para identificar a configuração de vários modos app para a configuração de quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3770f8c63be230dff97e43d3706ed35d79826751
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977126"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="b99a3-103">tipo de recurso de windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="b99a3-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="b99a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b99a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b99a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b99a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b99a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b99a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b99a3-107">A classe usada para identificar a configuração de vários modos app para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="b99a3-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>

<span data-ttu-id="b99a3-108">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b99a3-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b99a3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b99a3-109">Properties</span></span>
|<span data-ttu-id="b99a3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b99a3-110">Property</span></span>|<span data-ttu-id="b99a3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b99a3-111">Type</span></span>|<span data-ttu-id="b99a3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b99a3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b99a3-113">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="b99a3-113">apps</span></span>|<span data-ttu-id="b99a3-114">coleção [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="b99a3-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="b99a3-115">Estes são os únicos repositório aplicativos do Windows que estarão disponíveis para início no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="b99a3-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="b99a3-116">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="b99a3-116">showTaskBar</span></span>|<span data-ttu-id="b99a3-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="b99a3-117">Boolean</span></span>|<span data-ttu-id="b99a3-118">Essa configuração permite que o administrador especificar se a barra de tarefas é mostrada ou não.</span><span class="sxs-lookup"><span data-stu-id="b99a3-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="b99a3-119">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="b99a3-119">disallowDesktopApps</span></span>|<span data-ttu-id="b99a3-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="b99a3-120">Boolean</span></span>|<span data-ttu-id="b99a3-121">Essa configuração indica que os aplicativos da área de trabalho são permitidos.</span><span class="sxs-lookup"><span data-stu-id="b99a3-121">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="b99a3-122">Definido como true.</span><span class="sxs-lookup"><span data-stu-id="b99a3-122">Default to true.</span></span>|
|<span data-ttu-id="b99a3-123">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="b99a3-123">startMenuLayoutXml</span></span>|<span data-ttu-id="b99a3-124">Binária</span><span class="sxs-lookup"><span data-stu-id="b99a3-124">Binary</span></span>|<span data-ttu-id="b99a3-125">Permite que os administradores substituir o layout de início padrão e impede que o usuário alterá-la.</span><span class="sxs-lookup"><span data-stu-id="b99a3-125">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="b99a3-126">O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout.</span><span class="sxs-lookup"><span data-stu-id="b99a3-126"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="b99a3-127">XML deve estar em formato binário.</span><span class="sxs-lookup"><span data-stu-id="b99a3-127">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b99a3-128">Relações</span><span class="sxs-lookup"><span data-stu-id="b99a3-128">Relationships</span></span>
<span data-ttu-id="b99a3-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b99a3-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b99a3-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b99a3-130">JSON Representation</span></span>
<span data-ttu-id="b99a3-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b99a3-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```





