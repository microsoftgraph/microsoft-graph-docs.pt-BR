---
title: tipo de recurso win32LobAppRequirement
description: Classe base para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b32be470753f62b725b0cd1f91177ab8f1826d66
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422643"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="4fee4-103">tipo de recurso win32LobAppRequirement</span><span class="sxs-lookup"><span data-stu-id="4fee4-103">win32LobAppRequirement resource type</span></span>

<span data-ttu-id="4fee4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fee4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fee4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4fee4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fee4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fee4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fee4-107">Classe base para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="4fee4-107">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="4fee4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4fee4-108">Properties</span></span>
|<span data-ttu-id="4fee4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fee4-109">Property</span></span>|<span data-ttu-id="4fee4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fee4-110">Type</span></span>|<span data-ttu-id="4fee4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fee4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fee4-112">operator</span><span class="sxs-lookup"><span data-stu-id="4fee4-112">operator</span></span>|[<span data-ttu-id="4fee4-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="4fee4-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="4fee4-114">O operador para detecção.</span><span class="sxs-lookup"><span data-stu-id="4fee4-114">The operator for detection.</span></span> <span data-ttu-id="4fee4-115">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="4fee4-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="4fee4-116">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="4fee4-116">detectionValue</span></span>|<span data-ttu-id="4fee4-117">String</span><span class="sxs-lookup"><span data-stu-id="4fee4-117">String</span></span>|<span data-ttu-id="4fee4-118">O valor de detecção</span><span class="sxs-lookup"><span data-stu-id="4fee4-118">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fee4-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4fee4-119">Relationships</span></span>
<span data-ttu-id="4fee4-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4fee4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fee4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4fee4-121">JSON Representation</span></span>
<span data-ttu-id="4fee4-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4fee4-122">Here is a JSON representation of the resource.</span></span>
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



