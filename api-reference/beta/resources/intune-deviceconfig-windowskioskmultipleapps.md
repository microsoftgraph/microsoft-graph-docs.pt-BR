---
title: tipo de recurso tipo complexowindowskioskmultipleapps
description: A classe usada para identificar a configuração do aplicativo multimodo para a configuração do quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cae99ce452cdb9b002ebe4fe24968ec368c9fc0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783434"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="01bc7-103">tipo de recurso tipo complexowindowskioskmultipleapps</span><span class="sxs-lookup"><span data-stu-id="01bc7-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="01bc7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01bc7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01bc7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01bc7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01bc7-106">A classe usada para identificar a configuração do aplicativo multimodo para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="01bc7-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="01bc7-107">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bc7-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="01bc7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01bc7-108">Properties</span></span>
|<span data-ttu-id="01bc7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01bc7-109">Property</span></span>|<span data-ttu-id="01bc7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="01bc7-110">Type</span></span>|<span data-ttu-id="01bc7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="01bc7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01bc7-112">apps</span><span class="sxs-lookup"><span data-stu-id="01bc7-112">apps</span></span>|<span data-ttu-id="01bc7-113">coleção [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="01bc7-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="01bc7-114">Estes são os únicos aplicativos da Windows Store que estarão disponíveis para inicialização no menu iniciar.</span><span class="sxs-lookup"><span data-stu-id="01bc7-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="01bc7-115">Essa coleção pode conter um máximo de 128 elementos.</span><span class="sxs-lookup"><span data-stu-id="01bc7-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="01bc7-116">a barra de tarefas</span><span class="sxs-lookup"><span data-stu-id="01bc7-116">showTaskBar</span></span>|<span data-ttu-id="01bc7-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="01bc7-117">Boolean</span></span>|<span data-ttu-id="01bc7-118">Essa configuração permite que o administrador especifique se a barra de tarefas é mostrada ou não.</span><span class="sxs-lookup"><span data-stu-id="01bc7-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="01bc7-119">allowAccessToDownloadsFolder</span><span class="sxs-lookup"><span data-stu-id="01bc7-119">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="01bc7-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="01bc7-120">Boolean</span></span>|<span data-ttu-id="01bc7-121">Essa configuração permite o acesso à pasta downloads no explorador de arquivos.</span><span class="sxs-lookup"><span data-stu-id="01bc7-121">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="01bc7-122">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="01bc7-122">disallowDesktopApps</span></span>|<span data-ttu-id="01bc7-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="01bc7-123">Boolean</span></span>|<span data-ttu-id="01bc7-124">Essa configuração indica que os aplicativos de área de trabalho são permitidos.</span><span class="sxs-lookup"><span data-stu-id="01bc7-124">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="01bc7-125">O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="01bc7-125">Default to true.</span></span>|
|<span data-ttu-id="01bc7-126">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="01bc7-126">startMenuLayoutXml</span></span>|<span data-ttu-id="01bc7-127">Binária</span><span class="sxs-lookup"><span data-stu-id="01bc7-127">Binary</span></span>|<span data-ttu-id="01bc7-128">Permite que os administradores substituam o layout de início padrão e impede que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="01bc7-128">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="01bc7-129">O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout.</span><span class="sxs-lookup"><span data-stu-id="01bc7-129"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="01bc7-130">XML precisa estar no formato binário.</span><span class="sxs-lookup"><span data-stu-id="01bc7-130">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01bc7-131">Relações</span><span class="sxs-lookup"><span data-stu-id="01bc7-131">Relationships</span></span>
<span data-ttu-id="01bc7-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="01bc7-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01bc7-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01bc7-133">JSON Representation</span></span>
<span data-ttu-id="01bc7-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01bc7-134">Here is a JSON representation of the resource.</span></span>
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
      "appType": "String",
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```





