---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
ms.openlocfilehash: 4da5008eda31bb393ed25048c5d94724d2174e3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005153"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="2ce8a-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="2ce8a-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="2ce8a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2ce8a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ce8a-105">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="2ce8a-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="2ce8a-106">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="2ce8a-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ce8a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ce8a-107">Properties</span></span>
|<span data-ttu-id="2ce8a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ce8a-108">Property</span></span>|<span data-ttu-id="2ce8a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ce8a-109">Type</span></span>|<span data-ttu-id="2ce8a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ce8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ce8a-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="2ce8a-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="2ce8a-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="2ce8a-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="2ce8a-113">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="2ce8a-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="2ce8a-114">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="2ce8a-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ce8a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="2ce8a-115">Relationships</span></span>
<span data-ttu-id="2ce8a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ce8a-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ce8a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ce8a-117">JSON Representation</span></span>
<span data-ttu-id="2ce8a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ce8a-118">Here is a JSON representation of the resource.</span></span>
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



