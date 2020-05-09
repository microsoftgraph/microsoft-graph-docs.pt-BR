---
title: tipo de recurso deviceHealthScriptIntegerParameter
description: Propriedades do parâmetro de script Integer.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f88f027036c93b62610b9cd6d95821b5115a2334
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178560"
---
# <a name="devicehealthscriptintegerparameter-resource-type"></a><span data-ttu-id="82c64-103">tipo de recurso deviceHealthScriptIntegerParameter</span><span class="sxs-lookup"><span data-stu-id="82c64-103">deviceHealthScriptIntegerParameter resource type</span></span>

<span data-ttu-id="82c64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82c64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82c64-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82c64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82c64-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82c64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82c64-107">Propriedades do parâmetro de script Integer.</span><span class="sxs-lookup"><span data-stu-id="82c64-107">Properties of the  Integer script parameter.</span></span>


<span data-ttu-id="82c64-108">Herda de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="82c64-108">Inherits from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82c64-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82c64-109">Properties</span></span>
|<span data-ttu-id="82c64-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82c64-110">Property</span></span>|<span data-ttu-id="82c64-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="82c64-111">Type</span></span>|<span data-ttu-id="82c64-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="82c64-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82c64-113">name</span><span class="sxs-lookup"><span data-stu-id="82c64-113">name</span></span>|<span data-ttu-id="82c64-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82c64-114">String</span></span>|<span data-ttu-id="82c64-115">O nome do parâmetro herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="82c64-115">The name of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="82c64-116">description</span><span class="sxs-lookup"><span data-stu-id="82c64-116">description</span></span>|<span data-ttu-id="82c64-117">String</span><span class="sxs-lookup"><span data-stu-id="82c64-117">String</span></span>|<span data-ttu-id="82c64-118">A descrição do parâmetro herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="82c64-118">The description of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="82c64-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="82c64-119">isRequired</span></span>|<span data-ttu-id="82c64-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="82c64-120">Boolean</span></span>|<span data-ttu-id="82c64-121">Se o parâmetro obrigatório é herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="82c64-121">Whether the param is required Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="82c64-122">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="82c64-122">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="82c64-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="82c64-123">Boolean</span></span>|<span data-ttu-id="82c64-124">Se aplica DefaultValue quando não atribuído herdado de [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="82c64-124">Whether Apply DefaultValue When Not Assigned Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="82c64-125">defaultValue</span><span class="sxs-lookup"><span data-stu-id="82c64-125">defaultValue</span></span>|<span data-ttu-id="82c64-126">Int32</span><span class="sxs-lookup"><span data-stu-id="82c64-126">Int32</span></span>|<span data-ttu-id="82c64-127">O valor padrão do parâmetro Integer.</span><span class="sxs-lookup"><span data-stu-id="82c64-127">The default value of Integer param.</span></span> <span data-ttu-id="82c64-128">Valores válidos-2147483648 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="82c64-128">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="82c64-129">Relações</span><span class="sxs-lookup"><span data-stu-id="82c64-129">Relationships</span></span>
<span data-ttu-id="82c64-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82c64-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82c64-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82c64-131">JSON Representation</span></span>
<span data-ttu-id="82c64-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82c64-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptIntegerParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptIntegerParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true,
  "defaultValue": 1024
}
```



