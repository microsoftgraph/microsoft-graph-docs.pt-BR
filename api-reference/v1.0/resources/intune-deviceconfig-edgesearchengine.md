---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5ea2d73724400c033a3bd8e1148e04af8d390be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755067"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="3f4c0-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="3f4c0-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="3f4c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f4c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f4c0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f4c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f4c0-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="3f4c0-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="3f4c0-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="3f4c0-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f4c0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f4c0-108">Properties</span></span>
|<span data-ttu-id="3f4c0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f4c0-109">Property</span></span>|<span data-ttu-id="3f4c0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f4c0-110">Type</span></span>|<span data-ttu-id="3f4c0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f4c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f4c0-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="3f4c0-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="3f4c0-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="3f4c0-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="3f4c0-114">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="3f4c0-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="3f4c0-115">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="3f4c0-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f4c0-116">Relações</span><span class="sxs-lookup"><span data-stu-id="3f4c0-116">Relationships</span></span>
<span data-ttu-id="3f4c0-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3f4c0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f4c0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f4c0-118">JSON Representation</span></span>
<span data-ttu-id="3f4c0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f4c0-119">Here is a JSON representation of the resource.</span></span>
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




