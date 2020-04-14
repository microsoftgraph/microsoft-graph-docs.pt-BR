---
title: tipo de recurso deliveryOptimizationGroupIdCustom
description: Tipo de ID de grupo personalizado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d0b818a8c9e2a6a3cb13a8caa00b2115cf7f52b3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420476"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="12d7f-103">tipo de recurso deliveryOptimizationGroupIdCustom</span><span class="sxs-lookup"><span data-stu-id="12d7f-103">deliveryOptimizationGroupIdCustom resource type</span></span>

<span data-ttu-id="12d7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12d7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12d7f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12d7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12d7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12d7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12d7f-107">Tipo de ID de grupo personalizado</span><span class="sxs-lookup"><span data-stu-id="12d7f-107">Custom group id type</span></span>


<span data-ttu-id="12d7f-108">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="12d7f-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="12d7f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12d7f-109">Properties</span></span>
|<span data-ttu-id="12d7f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12d7f-110">Property</span></span>|<span data-ttu-id="12d7f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="12d7f-111">Type</span></span>|<span data-ttu-id="12d7f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="12d7f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12d7f-113">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="12d7f-113">groupIdCustom</span></span>|<span data-ttu-id="12d7f-114">String</span><span class="sxs-lookup"><span data-stu-id="12d7f-114">String</span></span>|<span data-ttu-id="12d7f-115">Especifica uma ID de grupo arbitrária à qual o dispositivo pertence</span><span class="sxs-lookup"><span data-stu-id="12d7f-115">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="12d7f-116">Relações</span><span class="sxs-lookup"><span data-stu-id="12d7f-116">Relationships</span></span>
<span data-ttu-id="12d7f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12d7f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12d7f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12d7f-118">JSON Representation</span></span>
<span data-ttu-id="12d7f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12d7f-119">Here is a JSON representation of the resource.</span></span>
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



