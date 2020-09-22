---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 040ff093004cdb1d31dde748a7ad26f03ce08b10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056790"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="ce727-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="ce727-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="ce727-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce727-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce727-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce727-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce727-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="ce727-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="ce727-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="ce727-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ce727-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce727-108">Properties</span></span>
|<span data-ttu-id="ce727-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce727-109">Property</span></span>|<span data-ttu-id="ce727-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce727-110">Type</span></span>|<span data-ttu-id="ce727-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce727-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce727-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="ce727-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="ce727-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="ce727-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="ce727-114">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="ce727-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="ce727-115">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="ce727-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce727-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ce727-116">Relationships</span></span>
<span data-ttu-id="ce727-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce727-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce727-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce727-118">JSON Representation</span></span>
<span data-ttu-id="ce727-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce727-119">Here is a JSON representation of the resource.</span></span>
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









