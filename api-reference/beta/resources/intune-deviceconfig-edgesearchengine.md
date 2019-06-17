---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1e44ee54752817b8dc95a1126a333d5065b507b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990229"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="aec49-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="aec49-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="aec49-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aec49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aec49-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aec49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aec49-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="aec49-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="aec49-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="aec49-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aec49-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aec49-108">Properties</span></span>
|<span data-ttu-id="aec49-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aec49-109">Property</span></span>|<span data-ttu-id="aec49-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="aec49-110">Type</span></span>|<span data-ttu-id="aec49-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aec49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aec49-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="aec49-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="aec49-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="aec49-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="aec49-114">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="aec49-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="aec49-115">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="aec49-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aec49-116">Relações</span><span class="sxs-lookup"><span data-stu-id="aec49-116">Relationships</span></span>
<span data-ttu-id="aec49-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aec49-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aec49-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aec49-118">JSON Representation</span></span>
<span data-ttu-id="aec49-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aec49-119">Here is a JSON representation of the resource.</span></span>
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





