---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f39793a781a0660da4295bd0c4d69b5b8b305987
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465663"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="0efcf-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="0efcf-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="0efcf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0efcf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0efcf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0efcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0efcf-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="0efcf-106">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="0efcf-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="0efcf-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0efcf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0efcf-108">Properties</span></span>
|<span data-ttu-id="0efcf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0efcf-109">Property</span></span>|<span data-ttu-id="0efcf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0efcf-110">Type</span></span>|<span data-ttu-id="0efcf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0efcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0efcf-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="0efcf-112">edgeSearchEngineType</span></span>|[<span data-ttu-id="0efcf-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="0efcf-113">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="0efcf-114">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="0efcf-114">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="0efcf-115">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="0efcf-115">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0efcf-116">Relações</span><span class="sxs-lookup"><span data-stu-id="0efcf-116">Relationships</span></span>
<span data-ttu-id="0efcf-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0efcf-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0efcf-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0efcf-118">JSON Representation</span></span>
<span data-ttu-id="0efcf-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0efcf-119">Here is a JSON representation of the resource.</span></span>
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







