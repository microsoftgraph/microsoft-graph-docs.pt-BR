---
title: Tipo de recurso edgeSearchEngine
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 619c925ff58745054a4cc62c638f1776ee96d5f2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199011"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="34a1b-103">Tipo de recurso edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="34a1b-103">edgeSearchEngine resource type</span></span>

<span data-ttu-id="34a1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34a1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34a1b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34a1b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34a1b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34a1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34a1b-107">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="34a1b-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="34a1b-108">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="34a1b-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34a1b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34a1b-109">Properties</span></span>
|<span data-ttu-id="34a1b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34a1b-110">Property</span></span>|<span data-ttu-id="34a1b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="34a1b-111">Type</span></span>|<span data-ttu-id="34a1b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="34a1b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34a1b-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="34a1b-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="34a1b-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="34a1b-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="34a1b-115">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão predefinido para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="34a1b-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="34a1b-116">Os valores possíveis são: `default`, `bing`.</span><span class="sxs-lookup"><span data-stu-id="34a1b-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34a1b-117">Relações</span><span class="sxs-lookup"><span data-stu-id="34a1b-117">Relationships</span></span>
<span data-ttu-id="34a1b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34a1b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34a1b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34a1b-119">JSON Representation</span></span>
<span data-ttu-id="34a1b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34a1b-120">Here is a JSON representation of the resource.</span></span>
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




