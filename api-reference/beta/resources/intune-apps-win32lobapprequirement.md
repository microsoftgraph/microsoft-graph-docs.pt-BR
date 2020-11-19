---
title: tipo de recurso win32LobAppRequirement
description: Classe base para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76f907b9eefe8d9b62aca05bc27dd92d7c8f61cd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280722"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="10b0e-103">tipo de recurso win32LobAppRequirement</span><span class="sxs-lookup"><span data-stu-id="10b0e-103">win32LobAppRequirement resource type</span></span>

<span data-ttu-id="10b0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10b0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10b0e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10b0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10b0e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10b0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10b0e-107">Classe base para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="10b0e-107">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="10b0e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10b0e-108">Properties</span></span>
|<span data-ttu-id="10b0e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10b0e-109">Property</span></span>|<span data-ttu-id="10b0e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="10b0e-110">Type</span></span>|<span data-ttu-id="10b0e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="10b0e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10b0e-112">operator</span><span class="sxs-lookup"><span data-stu-id="10b0e-112">operator</span></span>|[<span data-ttu-id="10b0e-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="10b0e-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="10b0e-114">O operador para detecção.</span><span class="sxs-lookup"><span data-stu-id="10b0e-114">The operator for detection.</span></span> <span data-ttu-id="10b0e-115">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="10b0e-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="10b0e-116">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="10b0e-116">detectionValue</span></span>|<span data-ttu-id="10b0e-117">String</span><span class="sxs-lookup"><span data-stu-id="10b0e-117">String</span></span>|<span data-ttu-id="10b0e-118">O valor de detecção</span><span class="sxs-lookup"><span data-stu-id="10b0e-118">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="10b0e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="10b0e-119">Relationships</span></span>
<span data-ttu-id="10b0e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10b0e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10b0e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10b0e-121">JSON Representation</span></span>
<span data-ttu-id="10b0e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10b0e-122">Here is a JSON representation of the resource.</span></span>
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




