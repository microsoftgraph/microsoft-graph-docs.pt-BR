---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7a58cbed251773559beb2589893ab9759d4758fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819905"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="30225-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="30225-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="30225-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="30225-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30225-105">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="30225-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="30225-106">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="30225-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="30225-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30225-107">Properties</span></span>
|<span data-ttu-id="30225-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30225-108">Property</span></span>|<span data-ttu-id="30225-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="30225-109">Type</span></span>|<span data-ttu-id="30225-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="30225-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30225-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="30225-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="30225-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="30225-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="30225-113">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="30225-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="30225-114">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="30225-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30225-115">Relações</span><span class="sxs-lookup"><span data-stu-id="30225-115">Relationships</span></span>
<span data-ttu-id="30225-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="30225-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30225-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30225-117">JSON Representation</span></span>
<span data-ttu-id="30225-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30225-118">Here is a JSON representation of the resource.</span></span>
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



