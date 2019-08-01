---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d733abca0dd390e83e51b25afd1ba7e86886b3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028375"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="cf7c4-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="cf7c4-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="cf7c4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf7c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf7c4-105">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="cf7c4-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="cf7c4-106">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="cf7c4-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cf7c4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf7c4-107">Properties</span></span>
|<span data-ttu-id="cf7c4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf7c4-108">Property</span></span>|<span data-ttu-id="cf7c4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf7c4-109">Type</span></span>|<span data-ttu-id="cf7c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf7c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf7c4-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="cf7c4-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="cf7c4-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="cf7c4-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="cf7c4-113">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="cf7c4-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="cf7c4-114">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="cf7c4-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf7c4-115">Relações</span><span class="sxs-lookup"><span data-stu-id="cf7c4-115">Relationships</span></span>
<span data-ttu-id="cf7c4-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf7c4-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf7c4-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf7c4-117">JSON Representation</span></span>
<span data-ttu-id="cf7c4-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf7c4-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



