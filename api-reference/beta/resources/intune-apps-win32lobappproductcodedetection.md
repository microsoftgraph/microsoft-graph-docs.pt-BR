---
title: tipo de recurso de win32LobAppProductCodeDetection
description: Contém propriedades de código e a versão do produto para detectar um aplicativo Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f5af1cfc5fffe5241ef3b7883c3ebe6a2100278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411201"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="0dcec-103">tipo de recurso de win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="0dcec-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="0dcec-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0dcec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0dcec-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0dcec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0dcec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0dcec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dcec-107">Contém propriedades de código e a versão do produto para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="0dcec-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="0dcec-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="0dcec-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0dcec-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0dcec-109">Properties</span></span>
|<span data-ttu-id="0dcec-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0dcec-110">Property</span></span>|<span data-ttu-id="0dcec-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0dcec-111">Type</span></span>|<span data-ttu-id="0dcec-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dcec-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dcec-113">productCode</span><span class="sxs-lookup"><span data-stu-id="0dcec-113">productCode</span></span>|<span data-ttu-id="0dcec-114">String</span><span class="sxs-lookup"><span data-stu-id="0dcec-114">String</span></span>|<span data-ttu-id="0dcec-115">O código do produto do aplicativo Win32 linha de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="0dcec-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0dcec-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="0dcec-116">productVersionOperator</span></span>|[<span data-ttu-id="0dcec-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="0dcec-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="0dcec-118">O operador para detectar a versão do produto.</span><span class="sxs-lookup"><span data-stu-id="0dcec-118">The operator to detect product version.</span></span> <span data-ttu-id="0dcec-119">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="0dcec-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="0dcec-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="0dcec-120">productVersion</span></span>|<span data-ttu-id="0dcec-121">String</span><span class="sxs-lookup"><span data-stu-id="0dcec-121">String</span></span>|<span data-ttu-id="0dcec-122">A versão de produto do aplicativo do Win32 linha de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="0dcec-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dcec-123">Relações</span><span class="sxs-lookup"><span data-stu-id="0dcec-123">Relationships</span></span>
<span data-ttu-id="0dcec-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0dcec-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dcec-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0dcec-125">JSON Representation</span></span>
<span data-ttu-id="0dcec-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0dcec-126">Here is a JSON representation of the resource.</span></span>
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




