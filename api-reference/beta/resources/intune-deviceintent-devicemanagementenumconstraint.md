---
title: tipo de recurso deviceManagementEnumConstraint
description: A restrição que impõe o valor da configuração é de um conjunto de cadeias de caracteres permitido
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 202365368c17d22cf33ea78320ac2a2604a59194
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061473"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="5b034-103">tipo de recurso deviceManagementEnumConstraint</span><span class="sxs-lookup"><span data-stu-id="5b034-103">deviceManagementEnumConstraint resource type</span></span>

<span data-ttu-id="5b034-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b034-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b034-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b034-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b034-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b034-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b034-107">A restrição que impõe o valor da configuração é de um conjunto de cadeias de caracteres permitido</span><span class="sxs-lookup"><span data-stu-id="5b034-107">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="5b034-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5b034-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b034-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b034-109">Properties</span></span>
|<span data-ttu-id="5b034-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b034-110">Property</span></span>|<span data-ttu-id="5b034-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b034-111">Type</span></span>|<span data-ttu-id="5b034-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b034-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b034-113">values</span><span class="sxs-lookup"><span data-stu-id="5b034-113">values</span></span>|<span data-ttu-id="5b034-114">coleção [deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5b034-114">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="5b034-115">Lista de valores válidos para esta cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b034-115">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b034-116">Relações</span><span class="sxs-lookup"><span data-stu-id="5b034-116">Relationships</span></span>
<span data-ttu-id="5b034-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b034-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b034-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b034-118">JSON Representation</span></span>
<span data-ttu-id="5b034-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b034-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumConstraint",
  "values": [
    {
      "@odata.type": "microsoft.graph.deviceManagementEnumValue",
      "value": "String",
      "displayName": "String"
    }
  ]
}
```






