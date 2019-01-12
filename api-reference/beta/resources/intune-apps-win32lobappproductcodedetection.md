---
title: tipo de recurso de win32LobAppProductCodeDetection
description: Contém propriedades de código e a versão do produto para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5536384178ac197d3b52609cb767fef82befd3b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928520"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="2814b-103">tipo de recurso de win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="2814b-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="2814b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2814b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2814b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2814b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2814b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2814b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2814b-107">Contém propriedades de código e a versão do produto para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="2814b-107">Contains product code and version properties to detect a Win32 App</span></span>

<span data-ttu-id="2814b-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="2814b-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2814b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2814b-109">Properties</span></span>
|<span data-ttu-id="2814b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2814b-110">Property</span></span>|<span data-ttu-id="2814b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2814b-111">Type</span></span>|<span data-ttu-id="2814b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2814b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2814b-113">productCode</span><span class="sxs-lookup"><span data-stu-id="2814b-113">productCode</span></span>|<span data-ttu-id="2814b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2814b-114">String</span></span>|<span data-ttu-id="2814b-115">O código do produto do aplicativo Win32 linha de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="2814b-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2814b-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="2814b-116">productVersionOperator</span></span>|[<span data-ttu-id="2814b-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="2814b-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="2814b-118">O operador para detectar a versão do produto.</span><span class="sxs-lookup"><span data-stu-id="2814b-118">The operator to detect product version.</span></span> <span data-ttu-id="2814b-119">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="2814b-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="2814b-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="2814b-120">productVersion</span></span>|<span data-ttu-id="2814b-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2814b-121">String</span></span>|<span data-ttu-id="2814b-122">A versão de produto do aplicativo do Win32 linha de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="2814b-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2814b-123">Relações</span><span class="sxs-lookup"><span data-stu-id="2814b-123">Relationships</span></span>
<span data-ttu-id="2814b-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2814b-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2814b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2814b-125">JSON Representation</span></span>
<span data-ttu-id="2814b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2814b-126">Here is a JSON representation of the resource.</span></span>
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





