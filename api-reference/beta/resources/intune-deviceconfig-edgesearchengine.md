---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
ms.openlocfilehash: 51f947911e73927816eb4f1150cab36cba904f58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033164"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="c9d1f-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="c9d1f-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="c9d1f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9d1f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9d1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9d1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9d1f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c9d1f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9d1f-107">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="c9d1f-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="c9d1f-108">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="c9d1f-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9d1f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9d1f-109">Properties</span></span>
|<span data-ttu-id="c9d1f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9d1f-110">Property</span></span>|<span data-ttu-id="c9d1f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9d1f-111">Type</span></span>|<span data-ttu-id="c9d1f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9d1f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9d1f-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c9d1f-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="c9d1f-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c9d1f-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="c9d1f-115">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="c9d1f-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="c9d1f-116">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="c9d1f-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9d1f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="c9d1f-117">Relationships</span></span>
<span data-ttu-id="c9d1f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9d1f-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9d1f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9d1f-119">JSON Representation</span></span>
<span data-ttu-id="c9d1f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9d1f-120">Here is a JSON representation of the resource.</span></span>
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





