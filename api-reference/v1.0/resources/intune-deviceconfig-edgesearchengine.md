---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 87a072ca6fb325f599c51a219bfa0e9d2ad0ac0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935616"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="a6f64-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="a6f64-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="a6f64-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a6f64-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6f64-105">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="a6f64-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="a6f64-106">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="a6f64-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a6f64-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6f64-107">Properties</span></span>
|<span data-ttu-id="a6f64-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6f64-108">Property</span></span>|<span data-ttu-id="a6f64-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6f64-109">Type</span></span>|<span data-ttu-id="a6f64-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6f64-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6f64-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a6f64-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="a6f64-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a6f64-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="a6f64-113">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="a6f64-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="a6f64-114">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="a6f64-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6f64-115">Relações</span><span class="sxs-lookup"><span data-stu-id="a6f64-115">Relationships</span></span>
<span data-ttu-id="a6f64-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6f64-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a6f64-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6f64-117">JSON Representation</span></span>
<span data-ttu-id="a6f64-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6f64-118">Here is a JSON representation of the resource.</span></span>
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



