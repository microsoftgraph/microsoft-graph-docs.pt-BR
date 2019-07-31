---
title: tipo de recurso win32LobAppProductCodeDetection
description: Contém as propriedades de código e versão do produto para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f8039c8ecd4e11774c78d349e6d9166c8e511bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004999"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="f9095-103">tipo de recurso win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="f9095-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="f9095-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9095-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9095-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9095-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9095-106">Contém as propriedades de código e versão do produto para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="f9095-106">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="f9095-107">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="f9095-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f9095-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9095-108">Properties</span></span>
|<span data-ttu-id="f9095-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9095-109">Property</span></span>|<span data-ttu-id="f9095-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9095-110">Type</span></span>|<span data-ttu-id="f9095-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9095-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9095-112">productCode</span><span class="sxs-lookup"><span data-stu-id="f9095-112">productCode</span></span>|<span data-ttu-id="f9095-113">String</span><span class="sxs-lookup"><span data-stu-id="f9095-113">String</span></span>|<span data-ttu-id="f9095-114">O código de produto do aplicativo de linha de negócios (LoB) Win32.</span><span class="sxs-lookup"><span data-stu-id="f9095-114">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f9095-115">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="f9095-115">productVersionOperator</span></span>|[<span data-ttu-id="f9095-116">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="f9095-116">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="f9095-117">O operador para detectar a versão do produto.</span><span class="sxs-lookup"><span data-stu-id="f9095-117">The operator to detect product version.</span></span> <span data-ttu-id="f9095-118">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="f9095-118">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="f9095-119">productVersion</span><span class="sxs-lookup"><span data-stu-id="f9095-119">productVersion</span></span>|<span data-ttu-id="f9095-120">String</span><span class="sxs-lookup"><span data-stu-id="f9095-120">String</span></span>|<span data-ttu-id="f9095-121">A versão do produto do aplicativo de linha de negócios (LoB) Win32.</span><span class="sxs-lookup"><span data-stu-id="f9095-121">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9095-122">Relações</span><span class="sxs-lookup"><span data-stu-id="f9095-122">Relationships</span></span>
<span data-ttu-id="f9095-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9095-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9095-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9095-124">JSON Representation</span></span>
<span data-ttu-id="f9095-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9095-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```





