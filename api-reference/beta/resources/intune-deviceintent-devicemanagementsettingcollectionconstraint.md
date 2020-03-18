---
title: tipo de recurso deviceManagementSettingCollectionConstraint
description: Restrição que impõe o número máximo de elementos de uma coleção
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 180d199997f288945ba9be282ebd7c2bdbee31ec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785355"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="fc2f2-103">tipo de recurso deviceManagementSettingCollectionConstraint</span><span class="sxs-lookup"><span data-stu-id="fc2f2-103">deviceManagementSettingCollectionConstraint resource type</span></span>

> <span data-ttu-id="fc2f2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc2f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc2f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc2f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc2f2-106">Restrição que impõe o número máximo de elementos de uma coleção</span><span class="sxs-lookup"><span data-stu-id="fc2f2-106">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="fc2f2-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="fc2f2-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc2f2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc2f2-108">Properties</span></span>
|<span data-ttu-id="fc2f2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc2f2-109">Property</span></span>|<span data-ttu-id="fc2f2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc2f2-110">Type</span></span>|<span data-ttu-id="fc2f2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc2f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc2f2-112">minimumLength</span><span class="sxs-lookup"><span data-stu-id="fc2f2-112">minimumLength</span></span>|<span data-ttu-id="fc2f2-113">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f2-113">Int32</span></span>|<span data-ttu-id="fc2f2-114">O número mínimo de elementos na coleção</span><span class="sxs-lookup"><span data-stu-id="fc2f2-114">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="fc2f2-115">maximumLength</span><span class="sxs-lookup"><span data-stu-id="fc2f2-115">maximumLength</span></span>|<span data-ttu-id="fc2f2-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2f2-116">Int32</span></span>|<span data-ttu-id="fc2f2-117">O número máximo de elementos na coleção</span><span class="sxs-lookup"><span data-stu-id="fc2f2-117">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc2f2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="fc2f2-118">Relationships</span></span>
<span data-ttu-id="fc2f2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc2f2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc2f2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc2f2-120">JSON Representation</span></span>
<span data-ttu-id="fc2f2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc2f2-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingCollectionConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCollectionConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```



