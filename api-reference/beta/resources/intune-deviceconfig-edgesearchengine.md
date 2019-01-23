---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b868be9ff34e85516e34040cb3ccb6f0efb95cb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402367"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="dc5ee-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="dc5ee-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="dc5ee-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="dc5ee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dc5ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dc5ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc5ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="dc5ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc5ee-107">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="dc5ee-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="dc5ee-108">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="dc5ee-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dc5ee-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc5ee-109">Properties</span></span>
|<span data-ttu-id="dc5ee-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc5ee-110">Property</span></span>|<span data-ttu-id="dc5ee-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc5ee-111">Type</span></span>|<span data-ttu-id="dc5ee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc5ee-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc5ee-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="dc5ee-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="dc5ee-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="dc5ee-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="dc5ee-115">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="dc5ee-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="dc5ee-116">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="dc5ee-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc5ee-117">Relações</span><span class="sxs-lookup"><span data-stu-id="dc5ee-117">Relationships</span></span>
<span data-ttu-id="dc5ee-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc5ee-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc5ee-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc5ee-119">JSON Representation</span></span>
<span data-ttu-id="dc5ee-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc5ee-120">Here is a JSON representation of the resource.</span></span>
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




