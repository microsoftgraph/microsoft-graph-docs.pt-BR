---
title: tipo de recurso deliveryOptimizationGroupIdSourceOptions
description: Tipo de opções de ID de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6d549c6f1601921e602a7fc51466e589109b0cc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199424"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="f54b4-103">tipo de recurso deliveryOptimizationGroupIdSourceOptions</span><span class="sxs-lookup"><span data-stu-id="f54b4-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

<span data-ttu-id="f54b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f54b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f54b4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f54b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f54b4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f54b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f54b4-107">Tipo de opções de ID de grupo</span><span class="sxs-lookup"><span data-stu-id="f54b4-107">Group id options type</span></span>


<span data-ttu-id="f54b4-108">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="f54b4-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f54b4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f54b4-109">Properties</span></span>
|<span data-ttu-id="f54b4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f54b4-110">Property</span></span>|<span data-ttu-id="f54b4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f54b4-111">Type</span></span>|<span data-ttu-id="f54b4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f54b4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f54b4-113">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="f54b4-113">groupIdSourceOption</span></span>|[<span data-ttu-id="f54b4-114">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="f54b4-114">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="f54b4-115">Defina essa política para restringir a seleção de par para uma fonte específica.</span><span class="sxs-lookup"><span data-stu-id="f54b4-115">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="f54b4-116">Os valores possíveis são: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span><span class="sxs-lookup"><span data-stu-id="f54b4-116">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f54b4-117">Relações</span><span class="sxs-lookup"><span data-stu-id="f54b4-117">Relationships</span></span>
<span data-ttu-id="f54b4-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f54b4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f54b4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f54b4-119">JSON Representation</span></span>
<span data-ttu-id="f54b4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f54b4-120">Here is a JSON representation of the resource.</span></span>
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




