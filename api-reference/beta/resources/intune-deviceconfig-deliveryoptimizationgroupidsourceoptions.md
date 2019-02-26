---
title: tipo de recurso deliveryOptimizationGroupIdSourceOptions
description: Tipo de opções de ID de grupo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d54a98bef3b9c0e0517b426332b8d3223e904c8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177851"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="4690b-103">tipo de recurso deliveryOptimizationGroupIdSourceOptions</span><span class="sxs-lookup"><span data-stu-id="4690b-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="4690b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4690b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4690b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4690b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4690b-106">Tipo de opções de ID de grupo</span><span class="sxs-lookup"><span data-stu-id="4690b-106">Group id options type</span></span>


<span data-ttu-id="4690b-107">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="4690b-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4690b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4690b-108">Properties</span></span>
|<span data-ttu-id="4690b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4690b-109">Property</span></span>|<span data-ttu-id="4690b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4690b-110">Type</span></span>|<span data-ttu-id="4690b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4690b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4690b-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="4690b-112">groupIdSourceOption</span></span>|[<span data-ttu-id="4690b-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="4690b-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="4690b-114">Defina essa política para restringir a seleção de par para uma fonte específica.</span><span class="sxs-lookup"><span data-stu-id="4690b-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="4690b-115">Os valores possíveis são: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span><span class="sxs-lookup"><span data-stu-id="4690b-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4690b-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4690b-116">Relationships</span></span>
<span data-ttu-id="4690b-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4690b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4690b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4690b-118">JSON Representation</span></span>
<span data-ttu-id="4690b-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4690b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSourceOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdSourceOptions",
  "groupIdSourceOption": "String"
}
```




