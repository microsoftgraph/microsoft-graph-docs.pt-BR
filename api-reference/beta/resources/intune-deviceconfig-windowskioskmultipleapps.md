---
title: tipo de recurso de windowsKioskMultipleApps
description: A classe usada para identificar a configuração de vários modos app para a configuração de quiosque
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71b8a57151b08d0297a89dfd815f72d66c2d12a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396025"
---
# <a name="windowskioskmultipleapps-resource-type"></a><span data-ttu-id="e599d-103">tipo de recurso de windowsKioskMultipleApps</span><span class="sxs-lookup"><span data-stu-id="e599d-103">windowsKioskMultipleApps resource type</span></span>

> <span data-ttu-id="e599d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e599d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e599d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e599d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e599d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e599d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e599d-107">A classe usada para identificar a configuração de vários modos app para a configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="e599d-107">The class used to identify the MultiMode app configuration for the kiosk configuration</span></span>


<span data-ttu-id="e599d-108">Herda de [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e599d-108">Inherits from [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e599d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e599d-109">Properties</span></span>
|<span data-ttu-id="e599d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e599d-110">Property</span></span>|<span data-ttu-id="e599d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e599d-111">Type</span></span>|<span data-ttu-id="e599d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e599d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e599d-113">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="e599d-113">apps</span></span>|<span data-ttu-id="e599d-114">coleção [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)</span><span class="sxs-lookup"><span data-stu-id="e599d-114">[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) collection</span></span>|<span data-ttu-id="e599d-115">Estes são os únicos repositório aplicativos do Windows que estarão disponíveis para início no menu Iniciar.</span><span class="sxs-lookup"><span data-stu-id="e599d-115">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span> <span data-ttu-id="e599d-116">Essa coleção pode conter um máximo de 128 elementos.</span><span class="sxs-lookup"><span data-stu-id="e599d-116">This collection can contain a maximum of 128 elements.</span></span>|
|<span data-ttu-id="e599d-117">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="e599d-117">showTaskBar</span></span>|<span data-ttu-id="e599d-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e599d-118">Boolean</span></span>|<span data-ttu-id="e599d-119">Essa configuração permite que o administrador especificar se a barra de tarefas é mostrada ou não.</span><span class="sxs-lookup"><span data-stu-id="e599d-119">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="e599d-120">disallowDesktopApps</span><span class="sxs-lookup"><span data-stu-id="e599d-120">disallowDesktopApps</span></span>|<span data-ttu-id="e599d-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="e599d-121">Boolean</span></span>|<span data-ttu-id="e599d-122">Essa configuração indica que os aplicativos da área de trabalho são permitidos.</span><span class="sxs-lookup"><span data-stu-id="e599d-122">This setting indicates that desktop apps are allowed.</span></span> <span data-ttu-id="e599d-123">Definido como true.</span><span class="sxs-lookup"><span data-stu-id="e599d-123">Default to true.</span></span>|
|<span data-ttu-id="e599d-124">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="e599d-124">startMenuLayoutXml</span></span>|<span data-ttu-id="e599d-125">Binária</span><span class="sxs-lookup"><span data-stu-id="e599d-125">Binary</span></span>|<span data-ttu-id="e599d-126">Permite que os administradores substituir o layout de início padrão e impede que o usuário alterá-la.</span><span class="sxs-lookup"><span data-stu-id="e599d-126">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="e599d-127">O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout.</span><span class="sxs-lookup"><span data-stu-id="e599d-127"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="e599d-128">XML deve estar em formato binário.</span><span class="sxs-lookup"><span data-stu-id="e599d-128">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e599d-129">Relações</span><span class="sxs-lookup"><span data-stu-id="e599d-129">Relationships</span></span>
<span data-ttu-id="e599d-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e599d-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e599d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e599d-131">JSON Representation</span></span>
<span data-ttu-id="e599d-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e599d-132">Here is a JSON representation of the resource.</span></span>
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




