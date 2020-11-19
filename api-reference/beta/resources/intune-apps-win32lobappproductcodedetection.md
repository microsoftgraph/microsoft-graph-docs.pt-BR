---
title: tipo de recurso win32LobAppProductCodeDetection
description: Contém as propriedades de código e versão do produto para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: baceeb2cbc3ddfe28e81871159fb24db96accd64
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280862"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="c416b-103">tipo de recurso win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="c416b-103">win32LobAppProductCodeDetection resource type</span></span>

<span data-ttu-id="c416b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c416b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c416b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c416b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c416b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c416b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c416b-107">Contém as propriedades de código e versão do produto para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="c416b-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="c416b-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="c416b-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c416b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c416b-109">Properties</span></span>
|<span data-ttu-id="c416b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c416b-110">Property</span></span>|<span data-ttu-id="c416b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c416b-111">Type</span></span>|<span data-ttu-id="c416b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c416b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c416b-113">productCode</span><span class="sxs-lookup"><span data-stu-id="c416b-113">productCode</span></span>|<span data-ttu-id="c416b-114">String</span><span class="sxs-lookup"><span data-stu-id="c416b-114">String</span></span>|<span data-ttu-id="c416b-115">O código de produto do aplicativo de linha de negócios (LoB) Win32.</span><span class="sxs-lookup"><span data-stu-id="c416b-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c416b-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="c416b-116">productVersionOperator</span></span>|[<span data-ttu-id="c416b-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="c416b-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="c416b-118">O operador para detectar a versão do produto.</span><span class="sxs-lookup"><span data-stu-id="c416b-118">The operator to detect product version.</span></span> <span data-ttu-id="c416b-119">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="c416b-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="c416b-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="c416b-120">productVersion</span></span>|<span data-ttu-id="c416b-121">String</span><span class="sxs-lookup"><span data-stu-id="c416b-121">String</span></span>|<span data-ttu-id="c416b-122">A versão do produto do aplicativo de linha de negócios (LoB) Win32.</span><span class="sxs-lookup"><span data-stu-id="c416b-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c416b-123">Relações</span><span class="sxs-lookup"><span data-stu-id="c416b-123">Relationships</span></span>
<span data-ttu-id="c416b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c416b-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c416b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c416b-125">JSON Representation</span></span>
<span data-ttu-id="c416b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c416b-126">Here is a JSON representation of the resource.</span></span>
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




