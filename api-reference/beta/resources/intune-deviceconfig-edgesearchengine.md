---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9808e5f1c51c6893159d1c04c1fae967e83cef64
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386171"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="2465f-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="2465f-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="2465f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2465f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2465f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2465f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2465f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2465f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2465f-107">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="2465f-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="2465f-108">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="2465f-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2465f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2465f-109">Properties</span></span>
|<span data-ttu-id="2465f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2465f-110">Property</span></span>|<span data-ttu-id="2465f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2465f-111">Type</span></span>|<span data-ttu-id="2465f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2465f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2465f-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="2465f-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="2465f-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="2465f-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="2465f-115">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="2465f-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="2465f-116">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="2465f-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2465f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="2465f-117">Relationships</span></span>
<span data-ttu-id="2465f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2465f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2465f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2465f-119">JSON Representation</span></span>
<span data-ttu-id="2465f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2465f-120">Here is a JSON representation of the resource.</span></span>
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



