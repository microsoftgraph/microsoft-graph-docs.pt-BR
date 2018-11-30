---
title: tipo de recurso de windowsKioskAppBase
description: A classe base para um tipo de aplicativos
ms.openlocfilehash: bbd2a961e86e698ff0b9a98401927c518beafe49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035474"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="26811-103">tipo de recurso de windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="26811-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="26811-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="26811-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26811-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="26811-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26811-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="26811-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26811-107">A classe base para um tipo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="26811-107">The base class for a type of apps</span></span>
## <a name="properties"></a><span data-ttu-id="26811-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26811-108">Properties</span></span>
|<span data-ttu-id="26811-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26811-109">Property</span></span>|<span data-ttu-id="26811-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="26811-110">Type</span></span>|<span data-ttu-id="26811-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26811-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26811-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="26811-112">startLayoutTileSize</span></span>|[<span data-ttu-id="26811-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="26811-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="26811-114">O tamanho de blocos de aplicativo para o layout de iniciar.</span><span class="sxs-lookup"><span data-stu-id="26811-114">The app tile size for the start layout.</span></span> <span data-ttu-id="26811-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="26811-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="26811-116">name</span><span class="sxs-lookup"><span data-stu-id="26811-116">name</span></span>|<span data-ttu-id="26811-117">String</span><span class="sxs-lookup"><span data-stu-id="26811-117">String</span></span>|<span data-ttu-id="26811-118">Representa o nome amigável de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="26811-118">Represents the friendly name of an app</span></span>|

## <a name="relationships"></a><span data-ttu-id="26811-119">Relações</span><span class="sxs-lookup"><span data-stu-id="26811-119">Relationships</span></span>
<span data-ttu-id="26811-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26811-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26811-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26811-121">JSON Representation</span></span>
<span data-ttu-id="26811-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26811-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String"
}
```





