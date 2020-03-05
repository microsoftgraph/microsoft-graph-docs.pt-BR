---
title: tipo de recurso deviceManagementEnumConstraint
description: A restrição que impõe o valor da configuração é de um conjunto de cadeias de caracteres permitido
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35dd4a8a4d69125e9bc675644980e5cfa3d90679
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525317"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="85c6a-103">tipo de recurso deviceManagementEnumConstraint</span><span class="sxs-lookup"><span data-stu-id="85c6a-103">deviceManagementEnumConstraint resource type</span></span>

<span data-ttu-id="85c6a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="85c6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85c6a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85c6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85c6a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85c6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85c6a-107">A restrição que impõe o valor da configuração é de um conjunto de cadeias de caracteres permitido</span><span class="sxs-lookup"><span data-stu-id="85c6a-107">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="85c6a-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="85c6a-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="85c6a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85c6a-109">Properties</span></span>
|<span data-ttu-id="85c6a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85c6a-110">Property</span></span>|<span data-ttu-id="85c6a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="85c6a-111">Type</span></span>|<span data-ttu-id="85c6a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="85c6a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85c6a-113">values</span><span class="sxs-lookup"><span data-stu-id="85c6a-113">values</span></span>|<span data-ttu-id="85c6a-114">coleção [deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md)</span><span class="sxs-lookup"><span data-stu-id="85c6a-114">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="85c6a-115">Lista de valores válidos para esta cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85c6a-115">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="85c6a-116">Relações</span><span class="sxs-lookup"><span data-stu-id="85c6a-116">Relationships</span></span>
<span data-ttu-id="85c6a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85c6a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85c6a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85c6a-118">JSON Representation</span></span>
<span data-ttu-id="85c6a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85c6a-119">Here is a JSON representation of the resource.</span></span>
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



