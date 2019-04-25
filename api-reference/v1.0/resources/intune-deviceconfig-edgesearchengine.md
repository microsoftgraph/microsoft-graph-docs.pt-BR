---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6867dd6b2243541b193b8b741924487f16ff61c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565972"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="e544b-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="e544b-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="e544b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e544b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e544b-105">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="e544b-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="e544b-106">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="e544b-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e544b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e544b-107">Properties</span></span>
|<span data-ttu-id="e544b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e544b-108">Property</span></span>|<span data-ttu-id="e544b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e544b-109">Type</span></span>|<span data-ttu-id="e544b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e544b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e544b-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="e544b-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="e544b-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="e544b-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="e544b-113">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="e544b-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="e544b-114">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="e544b-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e544b-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e544b-115">Relationships</span></span>
<span data-ttu-id="e544b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e544b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e544b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e544b-117">JSON Representation</span></span>
<span data-ttu-id="e544b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e544b-118">Here is a JSON representation of the resource.</span></span>
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



