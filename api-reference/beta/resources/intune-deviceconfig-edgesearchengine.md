---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a83965eb67762135eba3dcf1edf31fb4aec7827
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946725"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="4fade-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="4fade-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="4fade-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4fade-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fade-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fade-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fade-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="4fade-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="4fade-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="4fade-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4fade-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4fade-108">Properties</span></span>
|<span data-ttu-id="4fade-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fade-109">Property</span></span>|<span data-ttu-id="4fade-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fade-110">Type</span></span>|<span data-ttu-id="4fade-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fade-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fade-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="4fade-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="4fade-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="4fade-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="4fade-114">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="4fade-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="4fade-115">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="4fade-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fade-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4fade-116">Relationships</span></span>
<span data-ttu-id="4fade-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4fade-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fade-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4fade-118">JSON Representation</span></span>
<span data-ttu-id="4fade-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4fade-119">Here is a JSON representation of the resource.</span></span>
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




