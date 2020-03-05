---
title: tipo de recurso tipo complexowindowskioskmultipleapps
description: A classe usada para identificar a configuração do aplicativo multimodo para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f5a56f3717b3d03b4caf900005661e316fa3401
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525471"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="274e7-103">tipo de recurso tipo complexowindowskioskmultipleapps</span><span class="sxs-lookup"><span data-stu-id="274e7-103">windowsKioskMultipleApps resource type</span></span>

<span data-ttu-id="274e7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="274e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="274e7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="274e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="274e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="274e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="274e7-107">A classe usada para identificar a configuração do aplicativo multimodo para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="274e7-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="274e7-108">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="274e7-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="274e7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="274e7-109">Properties</span></span>
|<span data-ttu-id="274e7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="274e7-110">Property</span></span>|<span data-ttu-id="274e7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="274e7-111">Type</span></span>|<span data-ttu-id="274e7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="274e7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="274e7-113">apps</span><span class="sxs-lookup"><span data-stu-id="274e7-113">apps</span></span>|<span data-ttu-id="274e7-114">coleção [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="274e7-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="274e7-115">Estes são os únicos aplicativos da Windows Store que estarão disponíveis para inicialização no menu iniciar.</span><span class="sxs-lookup"><span data-stu-id="274e7-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="274e7-116">Essa coleção pode conter um máximo de 128 elementos.</span><span class="sxs-lookup"><span data-stu-id="274e7-116">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="274e7-117">a barra de tarefas</span><span class="sxs-lookup"><span data-stu-id="274e7-117">showTaskBar</span></span>|<span data-ttu-id="274e7-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="274e7-118">Boolean</span></span>|<span data-ttu-id="274e7-119">Essa configuração permite que o administrador especifique se a barra de tarefas é mostrada ou não.</span><span class="sxs-lookup"><span data-stu-id="274e7-119">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="274e7-120">allowAccessToDownloadsFolder</span><span class="sxs-lookup"><span data-stu-id="274e7-120">allowAccessToDownloadsFolder</span></span>|<span data-ttu-id="274e7-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="274e7-121">Boolean</span></span>|<span data-ttu-id="274e7-122">Essa configuração permite o acesso à pasta downloads no explorador de arquivos.</span><span class="sxs-lookup"><span data-stu-id="274e7-122">This setting allows access to Downloads folder in file explorer.</span></span>|
|<span data-ttu-id="274e7-123">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="274e7-123">disallowDesktopApps</span></span>|<span data-ttu-id="274e7-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="274e7-124">Boolean</span></span>|<span data-ttu-id="274e7-125">Essa configuração indica que os aplicativos de área de trabalho são permitidos.</span><span class="sxs-lookup"><span data-stu-id="274e7-125">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="274e7-126">O padrão é true.</span><span class="sxs-lookup"><span data-stu-id="274e7-126">Default to true.</span></span>|
|<span data-ttu-id="274e7-127">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="274e7-127">startMenuLayoutXml</span></span>|<span data-ttu-id="274e7-128">Binária</span><span class="sxs-lookup"><span data-stu-id="274e7-128">Binary</span></span>|<span data-ttu-id="274e7-129">Permite que os administradores substituam o layout de início padrão e impede que o usuário o altere.</span><span class="sxs-lookup"><span data-stu-id="274e7-129">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="274e7-130">O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout.</span><span class="sxs-lookup"><span data-stu-id="274e7-130"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="274e7-131">XML precisa estar no formato binário.</span><span class="sxs-lookup"><span data-stu-id="274e7-131">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="274e7-132">Relações</span><span class="sxs-lookup"><span data-stu-id="274e7-132">Relationships</span></span>
<span data-ttu-id="274e7-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="274e7-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="274e7-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="274e7-134">JSON Representation</span></span>
<span data-ttu-id="274e7-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="274e7-135">Here is a JSON representation of the resource.</span></span>
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



