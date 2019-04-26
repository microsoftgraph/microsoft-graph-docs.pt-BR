---
title: tipo de recurso deliveryOptimizationGroupIdSourceOptions
description: Tipo de opções de ID de grupo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cd541fd9ff3a91f40be1b6ccea67787cdad2567
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565804"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="a24cf-103">tipo de recurso deliveryOptimizationGroupIdSourceOptions</span><span class="sxs-lookup"><span data-stu-id="a24cf-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="a24cf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a24cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a24cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a24cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a24cf-106">Tipo de opções de ID de grupo</span><span class="sxs-lookup"><span data-stu-id="a24cf-106">Group id options type</span></span>


<span data-ttu-id="a24cf-107">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="a24cf-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a24cf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a24cf-108">Properties</span></span>
|<span data-ttu-id="a24cf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a24cf-109">Property</span></span>|<span data-ttu-id="a24cf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a24cf-110">Type</span></span>|<span data-ttu-id="a24cf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a24cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a24cf-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="a24cf-112">groupIdSourceOption</span></span>|[<span data-ttu-id="a24cf-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="a24cf-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="a24cf-114">Defina essa política para restringir a seleção de par para uma fonte específica.</span><span class="sxs-lookup"><span data-stu-id="a24cf-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="a24cf-115">Os valores possíveis são: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span><span class="sxs-lookup"><span data-stu-id="a24cf-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a24cf-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a24cf-116">Relationships</span></span>
<span data-ttu-id="a24cf-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a24cf-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a24cf-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a24cf-118">JSON Representation</span></span>
<span data-ttu-id="a24cf-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a24cf-119">Here is a JSON representation of the resource.</span></span>
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





