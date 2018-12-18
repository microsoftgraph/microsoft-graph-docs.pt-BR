---
title: tipo de recurso de windowsKioskAppBase
description: A classe base para um tipo de aplicativos
author: tfitzmac
ms.openlocfilehash: 2afccff07d15fa1f2dfeff6a4ae9029494faa521
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307445"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="b027b-103">tipo de recurso de windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="b027b-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="b027b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b027b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b027b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b027b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b027b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b027b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b027b-107">A classe base para um tipo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="b027b-107">The base class for a type of apps</span></span>
## <a name="properties"></a><span data-ttu-id="b027b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b027b-108">Properties</span></span>
|<span data-ttu-id="b027b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b027b-109">Property</span></span>|<span data-ttu-id="b027b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b027b-110">Type</span></span>|<span data-ttu-id="b027b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b027b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b027b-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="b027b-112">startLayoutTileSize</span></span>|[<span data-ttu-id="b027b-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="b027b-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="b027b-114">O tamanho de blocos de aplicativo para o layout de iniciar.</span><span class="sxs-lookup"><span data-stu-id="b027b-114">The app tile size for the start layout.</span></span> <span data-ttu-id="b027b-115">Os valores possíveis são: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="b027b-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="b027b-116">name</span><span class="sxs-lookup"><span data-stu-id="b027b-116">name</span></span>|<span data-ttu-id="b027b-117">String</span><span class="sxs-lookup"><span data-stu-id="b027b-117">String</span></span>|<span data-ttu-id="b027b-118">Representa o nome amigável de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="b027b-118">Represents the friendly name of an app</span></span>|

## <a name="relationships"></a><span data-ttu-id="b027b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b027b-119">Relationships</span></span>
<span data-ttu-id="b027b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b027b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b027b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b027b-121">JSON Representation</span></span>
<span data-ttu-id="b027b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b027b-122">Here is a JSON representation of the resource.</span></span>
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





