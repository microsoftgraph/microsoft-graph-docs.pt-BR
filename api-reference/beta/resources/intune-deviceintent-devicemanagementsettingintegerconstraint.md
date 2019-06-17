---
title: tipo de recurso deviceManagementSettingIntegerConstraint
description: Restrição que impõe o intervalo de valor permitido para uma configuração de inteiro
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8d934da42efdfed3f161e11c0fc9835191e2051
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984496"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="8cecc-103">tipo de recurso deviceManagementSettingIntegerConstraint</span><span class="sxs-lookup"><span data-stu-id="8cecc-103">deviceManagementSettingIntegerConstraint resource type</span></span>

> <span data-ttu-id="8cecc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cecc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cecc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cecc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cecc-106">Restrição que impõe o intervalo de valor permitido para uma configuração de inteiro</span><span class="sxs-lookup"><span data-stu-id="8cecc-106">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="8cecc-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="8cecc-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8cecc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cecc-108">Properties</span></span>
|<span data-ttu-id="8cecc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cecc-109">Property</span></span>|<span data-ttu-id="8cecc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cecc-110">Type</span></span>|<span data-ttu-id="8cecc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cecc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cecc-112">MinimumValue</span><span class="sxs-lookup"><span data-stu-id="8cecc-112">minimumValue</span></span>|<span data-ttu-id="8cecc-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8cecc-113">Int32</span></span>|<span data-ttu-id="8cecc-114">O valor mínimo permitido</span><span class="sxs-lookup"><span data-stu-id="8cecc-114">The minimum permitted value</span></span>|
|<span data-ttu-id="8cecc-115">MaximumValue</span><span class="sxs-lookup"><span data-stu-id="8cecc-115">maximumValue</span></span>|<span data-ttu-id="8cecc-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8cecc-116">Int32</span></span>|<span data-ttu-id="8cecc-117">O valor máximo permitido</span><span class="sxs-lookup"><span data-stu-id="8cecc-117">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cecc-118">Relações</span><span class="sxs-lookup"><span data-stu-id="8cecc-118">Relationships</span></span>
<span data-ttu-id="8cecc-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cecc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cecc-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cecc-120">JSON Representation</span></span>
<span data-ttu-id="8cecc-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cecc-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingIntegerConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingIntegerConstraint",
  "minimumValue": 1024,
  "maximumValue": 1024
}
```





