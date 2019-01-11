---
title: tipo de recurso de windowsKioskAppBase
description: A classe base para um tipo de aplicativos
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa83243959105b09707fa28a53271d8f95c5fd1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845154"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="981ac-103">tipo de recurso de windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="981ac-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="981ac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="981ac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="981ac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="981ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="981ac-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="981ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="981ac-107">A classe base para um tipo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="981ac-107">The base class for a type of apps</span></span>
## <a name="properties"></a><span data-ttu-id="981ac-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="981ac-108">Properties</span></span>
|<span data-ttu-id="981ac-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="981ac-109">Property</span></span>|<span data-ttu-id="981ac-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="981ac-110">Type</span></span>|<span data-ttu-id="981ac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="981ac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="981ac-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="981ac-112">startLayoutTileSize</span></span>|[<span data-ttu-id="981ac-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="981ac-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="981ac-114">O tamanho de blocos de aplicativo para o layout de iniciar.</span><span class="sxs-lookup"><span data-stu-id="981ac-114">The app tile size for the start layout.</span></span> <span data-ttu-id="981ac-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="981ac-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="981ac-116">name</span><span class="sxs-lookup"><span data-stu-id="981ac-116">name</span></span>|<span data-ttu-id="981ac-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="981ac-117">String</span></span>|<span data-ttu-id="981ac-118">Representa o nome amigável de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="981ac-118">Represents the friendly name of an app</span></span>|

## <a name="relationships"></a><span data-ttu-id="981ac-119">Relações</span><span class="sxs-lookup"><span data-stu-id="981ac-119">Relationships</span></span>
<span data-ttu-id="981ac-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="981ac-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="981ac-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="981ac-121">JSON Representation</span></span>
<span data-ttu-id="981ac-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="981ac-122">Here is a JSON representation of the resource.</span></span>
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





