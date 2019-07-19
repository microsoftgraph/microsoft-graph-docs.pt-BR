---
title: tipo de recurso deviceManagementEnumConstraint
description: A restrição que impõe o valor da configuração é de um conjunto de cadeias de caracteres permitido
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64c07f663d034cf6fa758155294730015ca6e3b4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964098"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="04fb2-103">tipo de recurso deviceManagementEnumConstraint</span><span class="sxs-lookup"><span data-stu-id="04fb2-103">deviceManagementEnumConstraint resource type</span></span>

> <span data-ttu-id="04fb2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04fb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04fb2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04fb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04fb2-106">A restrição que impõe o valor da configuração é de um conjunto de cadeias de caracteres permitido</span><span class="sxs-lookup"><span data-stu-id="04fb2-106">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="04fb2-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="04fb2-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04fb2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04fb2-108">Properties</span></span>
|<span data-ttu-id="04fb2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04fb2-109">Property</span></span>|<span data-ttu-id="04fb2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04fb2-110">Type</span></span>|<span data-ttu-id="04fb2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04fb2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04fb2-112">values</span><span class="sxs-lookup"><span data-stu-id="04fb2-112">values</span></span>|<span data-ttu-id="04fb2-113">coleção [deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md)</span><span class="sxs-lookup"><span data-stu-id="04fb2-113">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="04fb2-114">Lista de valores válidos para esta cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04fb2-114">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="04fb2-115">Relações</span><span class="sxs-lookup"><span data-stu-id="04fb2-115">Relationships</span></span>
<span data-ttu-id="04fb2-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04fb2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04fb2-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04fb2-117">JSON Representation</span></span>
<span data-ttu-id="04fb2-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04fb2-118">Here is a JSON representation of the resource.</span></span>
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





