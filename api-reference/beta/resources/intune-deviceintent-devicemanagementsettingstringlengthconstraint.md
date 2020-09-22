---
title: tipo de recurso deviceManagementSettingStringLengthConstraint
description: Restrição que impõe um determinado intervalo de duração da cadeia de caracteres
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 308bb7b723e9d8ac47bca72f342adb3f2a987ea5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061123"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="c748e-103">tipo de recurso deviceManagementSettingStringLengthConstraint</span><span class="sxs-lookup"><span data-stu-id="c748e-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

<span data-ttu-id="c748e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c748e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c748e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c748e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c748e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c748e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c748e-107">Restrição que impõe um determinado intervalo de duração da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c748e-107">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="c748e-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="c748e-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c748e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c748e-109">Properties</span></span>
|<span data-ttu-id="c748e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c748e-110">Property</span></span>|<span data-ttu-id="c748e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c748e-111">Type</span></span>|<span data-ttu-id="c748e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c748e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c748e-113">minimumLength</span><span class="sxs-lookup"><span data-stu-id="c748e-113">minimumLength</span></span>|<span data-ttu-id="c748e-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c748e-114">Int32</span></span>|<span data-ttu-id="c748e-115">O tamanho mínimo permitido da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c748e-115">The minimum permitted string length</span></span>|
|<span data-ttu-id="c748e-116">maximumLength</span><span class="sxs-lookup"><span data-stu-id="c748e-116">maximumLength</span></span>|<span data-ttu-id="c748e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="c748e-117">Int32</span></span>|<span data-ttu-id="c748e-118">O tamanho máximo permitido da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c748e-118">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="c748e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="c748e-119">Relationships</span></span>
<span data-ttu-id="c748e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c748e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c748e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c748e-121">JSON Representation</span></span>
<span data-ttu-id="c748e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c748e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingStringLengthConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingStringLengthConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```






