---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9828d2540f1b386302c18cde67811fe06fd9e50f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530044"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="91428-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="91428-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="91428-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="91428-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91428-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91428-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91428-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91428-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91428-107">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="91428-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="91428-108">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="91428-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91428-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91428-109">Properties</span></span>
|<span data-ttu-id="91428-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91428-110">Property</span></span>|<span data-ttu-id="91428-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="91428-111">Type</span></span>|<span data-ttu-id="91428-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="91428-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91428-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="91428-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="91428-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="91428-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="91428-115">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="91428-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="91428-116">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="91428-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91428-117">Relações</span><span class="sxs-lookup"><span data-stu-id="91428-117">Relationships</span></span>
<span data-ttu-id="91428-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91428-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91428-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91428-119">JSON Representation</span></span>
<span data-ttu-id="91428-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91428-120">Here is a JSON representation of the resource.</span></span>
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



