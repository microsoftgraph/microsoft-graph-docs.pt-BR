---
title: tipo de recurso deliveryOptimizationGroupIdSourceOptions
description: Tipo de opções de ID de grupo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 741b39245c26858d4cae46923d1078f568cf6945
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526769"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="8510c-103">tipo de recurso deliveryOptimizationGroupIdSourceOptions</span><span class="sxs-lookup"><span data-stu-id="8510c-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

<span data-ttu-id="8510c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8510c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8510c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8510c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8510c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8510c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8510c-107">Tipo de opções de ID de grupo</span><span class="sxs-lookup"><span data-stu-id="8510c-107">Group id options type</span></span>


<span data-ttu-id="8510c-108">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="8510c-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8510c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8510c-109">Properties</span></span>
|<span data-ttu-id="8510c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8510c-110">Property</span></span>|<span data-ttu-id="8510c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8510c-111">Type</span></span>|<span data-ttu-id="8510c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8510c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8510c-113">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="8510c-113">groupIdSourceOption</span></span>|[<span data-ttu-id="8510c-114">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="8510c-114">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="8510c-115">Defina essa política para restringir a seleção de par para uma fonte específica.</span><span class="sxs-lookup"><span data-stu-id="8510c-115">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="8510c-116">Os valores possíveis são: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span><span class="sxs-lookup"><span data-stu-id="8510c-116">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8510c-117">Relações</span><span class="sxs-lookup"><span data-stu-id="8510c-117">Relationships</span></span>
<span data-ttu-id="8510c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8510c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8510c-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8510c-119">JSON Representation</span></span>
<span data-ttu-id="8510c-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8510c-120">Here is a JSON representation of the resource.</span></span>
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



