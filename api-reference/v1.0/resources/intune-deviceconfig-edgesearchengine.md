---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1be131396c67f5af37a10ab3e0b7b1248cc8c4bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532544"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="5cd1d-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="5cd1d-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="5cd1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cd1d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cd1d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cd1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cd1d-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="5cd1d-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="5cd1d-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="5cd1d-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5cd1d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cd1d-108">Properties</span></span>
|<span data-ttu-id="5cd1d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cd1d-109">Property</span></span>|<span data-ttu-id="5cd1d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cd1d-110">Type</span></span>|<span data-ttu-id="5cd1d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cd1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cd1d-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="5cd1d-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="5cd1d-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="5cd1d-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="5cd1d-114">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="5cd1d-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="5cd1d-115">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="5cd1d-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cd1d-116">Relações</span><span class="sxs-lookup"><span data-stu-id="5cd1d-116">Relationships</span></span>
<span data-ttu-id="5cd1d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cd1d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cd1d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cd1d-118">JSON Representation</span></span>
<span data-ttu-id="5cd1d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cd1d-119">Here is a JSON representation of the resource.</span></span>
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




