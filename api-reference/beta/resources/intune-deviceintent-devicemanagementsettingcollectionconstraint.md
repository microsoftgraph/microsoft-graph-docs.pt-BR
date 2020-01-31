---
title: tipo de recurso deviceManagementSettingCollectionConstraint
description: Restrição que impõe o número máximo de elementos de uma coleção
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfad548881f4466cce4c4015506a342610c03b35
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636739"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="e421b-103">tipo de recurso deviceManagementSettingCollectionConstraint</span><span class="sxs-lookup"><span data-stu-id="e421b-103">deviceManagementSettingCollectionConstraint resource type</span></span>

> <span data-ttu-id="e421b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e421b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e421b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e421b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e421b-106">Restrição que impõe o número máximo de elementos de uma coleção</span><span class="sxs-lookup"><span data-stu-id="e421b-106">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="e421b-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e421b-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e421b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e421b-108">Properties</span></span>
|<span data-ttu-id="e421b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e421b-109">Property</span></span>|<span data-ttu-id="e421b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e421b-110">Type</span></span>|<span data-ttu-id="e421b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e421b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e421b-112">minimumLength</span><span class="sxs-lookup"><span data-stu-id="e421b-112">minimumLength</span></span>|<span data-ttu-id="e421b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e421b-113">Int32</span></span>|<span data-ttu-id="e421b-114">O número mínimo de elementos na coleção</span><span class="sxs-lookup"><span data-stu-id="e421b-114">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="e421b-115">maximumLength</span><span class="sxs-lookup"><span data-stu-id="e421b-115">maximumLength</span></span>|<span data-ttu-id="e421b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e421b-116">Int32</span></span>|<span data-ttu-id="e421b-117">O número máximo de elementos na coleção</span><span class="sxs-lookup"><span data-stu-id="e421b-117">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="e421b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e421b-118">Relationships</span></span>
<span data-ttu-id="e421b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e421b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e421b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e421b-120">JSON Representation</span></span>
<span data-ttu-id="e421b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e421b-121">Here is a JSON representation of the resource.</span></span>
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



