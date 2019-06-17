---
title: tipo de recurso deliveryOptimizationGroupIdCustom
description: Tipo de ID de grupo personalizado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3dbddceca6f6b7adc023431a8b8157ce02ef379
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979645"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="8f636-103">tipo de recurso deliveryOptimizationGroupIdCustom</span><span class="sxs-lookup"><span data-stu-id="8f636-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="8f636-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8f636-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f636-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f636-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f636-106">Tipo de ID de grupo personalizado</span><span class="sxs-lookup"><span data-stu-id="8f636-106">Custom group id type</span></span>


<span data-ttu-id="8f636-107">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="8f636-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8f636-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f636-108">Properties</span></span>
|<span data-ttu-id="8f636-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f636-109">Property</span></span>|<span data-ttu-id="8f636-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f636-110">Type</span></span>|<span data-ttu-id="8f636-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f636-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f636-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="8f636-112">groupIdCustom</span></span>|<span data-ttu-id="8f636-113">String</span><span class="sxs-lookup"><span data-stu-id="8f636-113">String</span></span>|<span data-ttu-id="8f636-114">Especifica uma ID de grupo arbitrária à qual o dispositivo pertence</span><span class="sxs-lookup"><span data-stu-id="8f636-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f636-115">Relações</span><span class="sxs-lookup"><span data-stu-id="8f636-115">Relationships</span></span>
<span data-ttu-id="8f636-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f636-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f636-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f636-117">JSON Representation</span></span>
<span data-ttu-id="8f636-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f636-118">Here is a JSON representation of the resource.</span></span>
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





