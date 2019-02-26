---
title: tipo de recurso deliveryOptimizationGroupIdCustom
description: Tipo de ID de grupo personalizado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3b00920d0ead3df5fe694e110825615f449ef4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177970"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="e8658-103">tipo de recurso deliveryOptimizationGroupIdCustom</span><span class="sxs-lookup"><span data-stu-id="e8658-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="e8658-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8658-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8658-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8658-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8658-106">Tipo de ID de grupo personalizado</span><span class="sxs-lookup"><span data-stu-id="e8658-106">Custom group id type</span></span>


<span data-ttu-id="e8658-107">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="e8658-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8658-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8658-108">Properties</span></span>
|<span data-ttu-id="e8658-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8658-109">Property</span></span>|<span data-ttu-id="e8658-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8658-110">Type</span></span>|<span data-ttu-id="e8658-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8658-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8658-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="e8658-112">groupIdCustom</span></span>|<span data-ttu-id="e8658-113">String</span><span class="sxs-lookup"><span data-stu-id="e8658-113">String</span></span>|<span data-ttu-id="e8658-114">Especifica uma ID de grupo arbitrária à qual o dispositivo pertence</span><span class="sxs-lookup"><span data-stu-id="e8658-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8658-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e8658-115">Relationships</span></span>
<span data-ttu-id="e8658-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8658-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8658-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8658-117">JSON Representation</span></span>
<span data-ttu-id="e8658-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8658-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```




