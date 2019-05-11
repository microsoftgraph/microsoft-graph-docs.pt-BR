---
title: tipo de recurso tipo complexowindowskioskmultipleapps
description: A classe usada para identificar a configuração do aplicativo multimodo para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df9fec1c5d21d7d23c5c7a56c3760b88348c556b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944002"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="0edc4-103">tipo de recurso tipo complexowindowskioskmultipleapps</span><span class="sxs-lookup"><span data-stu-id="0edc4-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="0edc4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0edc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0edc4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0edc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0edc4-106">A classe usada para identificar a configuração do aplicativo multimodo para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="0edc4-106">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="0edc4-107">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0edc4-107">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0edc4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0edc4-108">Properties</span></span>
|<span data-ttu-id="0edc4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0edc4-109">Property</span></span>|<span data-ttu-id="0edc4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0edc4-110">Type</span></span>|<span data-ttu-id="0edc4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0edc4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0edc4-112">apps</span><span class="sxs-lookup"><span data-stu-id="0edc4-112">apps</span></span>|<span data-ttu-id="0edc4-113">coleção [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="0edc4-113">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="0edc4-114">Estes são os únicos aplicativos da Windows Store que estarão disponíveis para inicialização no menu iniciar.</span><span class="sxs-lookup"><span data-stu-id="0edc4-114">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="0edc4-115">Essa coleção pode conter um máximo de 128 elementos.</span><span class="sxs-lookup"><span data-stu-id="0edc4-115">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="0edc4-116">a barra de tarefas</span><span class="sxs-lookup"><span data-stu-id="0edc4-116">showTaskBar</span></span>|<span data-ttu-id="0edc4-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="0edc4-117">Boolean</span></span>|<span data-ttu-id="0edc4-118">Essa configuração permite que o administrador especifique se a barra de tarefas é mostrada ou não.</span><span class="sxs-lookup"><span data-stu-id="0edc4-118">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="0edc4-119">allowAccessToDownloadsFolder</span><span class="sxs-lookup"><span data-stu-id="0edc4-119">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="0edc4-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="0edc4-120">Boolean</span></span>|<span data-ttu-id="0edc4-121">Essa configuração permite o acesso à pasta downloads no explorador de arquivos.</span><span class="sxs-lookup"><span data-stu-id="0edc4-121">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="0edc4-122">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="0edc4-122">disallowDesktopApps</span></span>|<span data-ttu-id="0edc4-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="0edc4-123">Boolean</span></span>|<span data-ttu-id="0edc4-124">Essa configuração indica que os aplicativos de área de trabalho são permitidos.</span><span class="sxs-lookup"><span data-stu-id="0edc4-124">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="0edc4-125">O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="0edc4-125">Default to true.</span></span>|
|<span data-ttu-id="0edc4-126">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="0edc4-126">startMenuLayoutXml</span></span>|<span data-ttu-id="0edc4-127">Binária</span><span class="sxs-lookup"><span data-stu-id="0edc4-127">Binary</span></span>|<span data-ttu-id="0edc4-128">Permite que os administradores substituam o layout de início padrão e impede que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="0edc4-128">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="0edc4-129">O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout.</span><span class="sxs-lookup"><span data-stu-id="0edc4-129"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="0edc4-130">XML precisa estar no formato binário.</span><span class="sxs-lookup"><span data-stu-id="0edc4-130">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0edc4-131">Relações</span><span class="sxs-lookup"><span data-stu-id="0edc4-131">Relationships</span></span>
<span data-ttu-id="0edc4-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0edc4-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0edc4-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0edc4-133">JSON Representation</span></span>
<span data-ttu-id="0edc4-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0edc4-134">Here is a JSON representation of the resource.</span></span>
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




