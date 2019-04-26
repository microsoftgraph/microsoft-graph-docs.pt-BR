---
title: tipo de recurso win32LobAppRequirement
description: Classe base para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3177493c5289b54cb43369a9dc62970097486f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554097"
---
# <a name="win32lobapprequirement-resource-type"></a><span data-ttu-id="9424d-103">tipo de recurso win32LobAppRequirement</span><span class="sxs-lookup"><span data-stu-id="9424d-103">win32LobAppRequirement resource type</span></span>

> <span data-ttu-id="9424d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9424d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9424d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9424d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9424d-106">Classe base para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="9424d-106">Base class to detect a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="9424d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9424d-107">Properties</span></span>
|<span data-ttu-id="9424d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9424d-108">Property</span></span>|<span data-ttu-id="9424d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9424d-109">Type</span></span>|<span data-ttu-id="9424d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9424d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9424d-111">operator</span><span class="sxs-lookup"><span data-stu-id="9424d-111">operator</span></span>|[<span data-ttu-id="9424d-112">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="9424d-112">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="9424d-113">O operador para detecção.</span><span class="sxs-lookup"><span data-stu-id="9424d-113">The operator for detection.</span></span> <span data-ttu-id="9424d-114">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="9424d-114">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="9424d-115">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="9424d-115">detectionValue</span></span>|<span data-ttu-id="9424d-116">String</span><span class="sxs-lookup"><span data-stu-id="9424d-116">String</span></span>|<span data-ttu-id="9424d-117">O valor de detecção</span><span class="sxs-lookup"><span data-stu-id="9424d-117">The detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="9424d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9424d-118">Relationships</span></span>
<span data-ttu-id="9424d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9424d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9424d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9424d-120">JSON Representation</span></span>
<span data-ttu-id="9424d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9424d-121">Here is a JSON representation of the resource.</span></span>
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





