---
title: tipo de recurso deviceManagementSettingCollectionConstraint
description: Restrição que impõe o número máximo de elementos de uma coleção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6bd64e29e01858ce6f1b09ef822e2a3621d5720
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061263"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="b549f-103">tipo de recurso deviceManagementSettingCollectionConstraint</span><span class="sxs-lookup"><span data-stu-id="b549f-103">deviceManagementSettingCollectionConstraint resource type</span></span>

<span data-ttu-id="b549f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b549f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b549f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b549f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b549f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b549f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b549f-107">Restrição que impõe o número máximo de elementos de uma coleção</span><span class="sxs-lookup"><span data-stu-id="b549f-107">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="b549f-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b549f-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b549f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b549f-109">Properties</span></span>
|<span data-ttu-id="b549f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b549f-110">Property</span></span>|<span data-ttu-id="b549f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b549f-111">Type</span></span>|<span data-ttu-id="b549f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b549f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b549f-113">minimumLength</span><span class="sxs-lookup"><span data-stu-id="b549f-113">minimumLength</span></span>|<span data-ttu-id="b549f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b549f-114">Int32</span></span>|<span data-ttu-id="b549f-115">O número mínimo de elementos na coleção</span><span class="sxs-lookup"><span data-stu-id="b549f-115">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="b549f-116">maximumLength</span><span class="sxs-lookup"><span data-stu-id="b549f-116">maximumLength</span></span>|<span data-ttu-id="b549f-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b549f-117">Int32</span></span>|<span data-ttu-id="b549f-118">O número máximo de elementos na coleção</span><span class="sxs-lookup"><span data-stu-id="b549f-118">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="b549f-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b549f-119">Relationships</span></span>
<span data-ttu-id="b549f-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b549f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b549f-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b549f-121">JSON Representation</span></span>
<span data-ttu-id="b549f-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b549f-122">Here is a JSON representation of the resource.</span></span>
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






