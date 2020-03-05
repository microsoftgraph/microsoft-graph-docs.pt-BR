---
title: tipo de recurso win32LobAppRequirement
description: Classe base para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9392c54dd78f0f7fce752423f9cf6c57a7713f58
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490340"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="9d448-103">tipo de recurso win32LobAppRequirement</span><span class="sxs-lookup"><span data-stu-id="9d448-103">win32LobAppRequirement resource type</span></span>

<span data-ttu-id="9d448-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9d448-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d448-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d448-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d448-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d448-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d448-107">Classe base para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="9d448-107">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="9d448-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d448-108">Properties</span></span>
|<span data-ttu-id="9d448-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d448-109">Property</span></span>|<span data-ttu-id="9d448-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d448-110">Type</span></span>|<span data-ttu-id="9d448-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d448-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d448-112">operator</span><span class="sxs-lookup"><span data-stu-id="9d448-112">operator</span></span>|[<span data-ttu-id="9d448-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="9d448-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="9d448-114">O operador para detecção.</span><span class="sxs-lookup"><span data-stu-id="9d448-114">The operator for detection.</span></span> <span data-ttu-id="9d448-115">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="9d448-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="9d448-116">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="9d448-116">detectionValue</span></span>|<span data-ttu-id="9d448-117">String</span><span class="sxs-lookup"><span data-stu-id="9d448-117">String</span></span>|<span data-ttu-id="9d448-118">O valor de detecção</span><span class="sxs-lookup"><span data-stu-id="9d448-118">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d448-119">Relações</span><span class="sxs-lookup"><span data-stu-id="9d448-119">Relationships</span></span>
<span data-ttu-id="9d448-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d448-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d448-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d448-121">JSON Representation</span></span>
<span data-ttu-id="9d448-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d448-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRequirement",
  "operator": "String",
  "detectionValue": "String"
}
```



