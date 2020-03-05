---
title: tipo de recurso deviceManagementSettingIntegerConstraint
description: Restrição que impõe o intervalo de valor permitido para uma configuração de inteiro
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c849d3a774535dd0cbf3e7628bcde2daa500fbe7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525233"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a><span data-ttu-id="d74ff-103">tipo de recurso deviceManagementSettingIntegerConstraint</span><span class="sxs-lookup"><span data-stu-id="d74ff-103">deviceManagementSettingIntegerConstraint resource type</span></span>

<span data-ttu-id="d74ff-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d74ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d74ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d74ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d74ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d74ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d74ff-107">Restrição que impõe o intervalo de valor permitido para uma configuração de inteiro</span><span class="sxs-lookup"><span data-stu-id="d74ff-107">Constraint enforcing the permitted value range for an integer setting</span></span>


<span data-ttu-id="d74ff-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d74ff-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d74ff-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d74ff-109">Properties</span></span>
|<span data-ttu-id="d74ff-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d74ff-110">Property</span></span>|<span data-ttu-id="d74ff-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d74ff-111">Type</span></span>|<span data-ttu-id="d74ff-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d74ff-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d74ff-113">MinimumValue</span><span class="sxs-lookup"><span data-stu-id="d74ff-113">minimumValue</span></span>|<span data-ttu-id="d74ff-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d74ff-114">Int32</span></span>|<span data-ttu-id="d74ff-115">O valor mínimo permitido</span><span class="sxs-lookup"><span data-stu-id="d74ff-115">The minimum permitted value</span></span>|
|<span data-ttu-id="d74ff-116">MaximumValue</span><span class="sxs-lookup"><span data-stu-id="d74ff-116">maximumValue</span></span>|<span data-ttu-id="d74ff-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d74ff-117">Int32</span></span>|<span data-ttu-id="d74ff-118">O valor máximo permitido</span><span class="sxs-lookup"><span data-stu-id="d74ff-118">The maximum permitted value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d74ff-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d74ff-119">Relationships</span></span>
<span data-ttu-id="d74ff-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d74ff-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d74ff-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d74ff-121">JSON Representation</span></span>
<span data-ttu-id="d74ff-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d74ff-122">Here is a JSON representation of the resource.</span></span>
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



