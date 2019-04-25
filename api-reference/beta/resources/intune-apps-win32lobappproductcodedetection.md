---
title: tipo de recurso win32LobAppProductCodeDetection
description: Contém as propriedades de código e versão do produto para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 755d0470873da1e5176e0962ace955d1fc647b80
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534462"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="57324-103">tipo de recurso win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="57324-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="57324-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57324-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57324-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57324-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57324-106">Contém as propriedades de código e versão do produto para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="57324-106">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="57324-107">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="57324-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57324-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57324-108">Properties</span></span>
|<span data-ttu-id="57324-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57324-109">Property</span></span>|<span data-ttu-id="57324-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="57324-110">Type</span></span>|<span data-ttu-id="57324-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="57324-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57324-112">productCode</span><span class="sxs-lookup"><span data-stu-id="57324-112">productCode</span></span>|<span data-ttu-id="57324-113">String</span><span class="sxs-lookup"><span data-stu-id="57324-113">String</span></span>|<span data-ttu-id="57324-114">O código de produto do aplicativo de linha de negócios (LoB) Win32.</span><span class="sxs-lookup"><span data-stu-id="57324-114">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="57324-115">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="57324-115">productVersionOperator</span></span>|[<span data-ttu-id="57324-116">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="57324-116">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="57324-117">O operador para detectar a versão do produto.</span><span class="sxs-lookup"><span data-stu-id="57324-117">The operator to detect product version.</span></span> <span data-ttu-id="57324-118">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="57324-118">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="57324-119">productVersion</span><span class="sxs-lookup"><span data-stu-id="57324-119">productVersion</span></span>|<span data-ttu-id="57324-120">String</span><span class="sxs-lookup"><span data-stu-id="57324-120">String</span></span>|<span data-ttu-id="57324-121">A versão do produto do aplicativo de linha de negócios (LoB) Win32.</span><span class="sxs-lookup"><span data-stu-id="57324-121">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57324-122">Relações</span><span class="sxs-lookup"><span data-stu-id="57324-122">Relationships</span></span>
<span data-ttu-id="57324-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57324-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57324-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57324-124">JSON Representation</span></span>
<span data-ttu-id="57324-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57324-125">Here is a JSON representation of the resource.</span></span>
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





