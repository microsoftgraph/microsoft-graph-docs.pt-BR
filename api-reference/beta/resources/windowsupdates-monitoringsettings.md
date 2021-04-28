---
title: Tipo de recurso monitoringSettings
description: Configurações controlar o monitoramento automatizado e a resposta em uma implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: aff5fa9571628783521dcc5ae0113e767915c2c7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067792"
---
# <a name="monitoringsettings-resource-type"></a><span data-ttu-id="14391-103">Tipo de recurso monitoringSettings</span><span class="sxs-lookup"><span data-stu-id="14391-103">monitoringSettings resource type</span></span>

<span data-ttu-id="14391-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="14391-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14391-105">Configurações controlar o monitoramento automatizado e a resposta em uma implantação.</span><span class="sxs-lookup"><span data-stu-id="14391-105">Settings controlling automated monitoring and response in a deployment.</span></span>

## <a name="properties"></a><span data-ttu-id="14391-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14391-106">Properties</span></span>
|<span data-ttu-id="14391-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14391-107">Property</span></span>|<span data-ttu-id="14391-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="14391-108">Type</span></span>|<span data-ttu-id="14391-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="14391-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14391-110">monitoringRules</span><span class="sxs-lookup"><span data-stu-id="14391-110">monitoringRules</span></span>|<span data-ttu-id="14391-111">[coleção microsoft.graph.windowsUpdates.monitoringRule](../resources/windowsupdates-monitoringrule.md)</span><span class="sxs-lookup"><span data-stu-id="14391-111">[microsoft.graph.windowsUpdates.monitoringRule](../resources/windowsupdates-monitoringrule.md) collection</span></span>|<span data-ttu-id="14391-112">Especifica as regras pelas quais os sinais de monitoramento podem disparar ações na implantação.</span><span class="sxs-lookup"><span data-stu-id="14391-112">Specifies the rules through which monitoring signals can trigger actions on the deployment.</span></span> <span data-ttu-id="14391-113">As regras são combinadas usando "ou".</span><span class="sxs-lookup"><span data-stu-id="14391-113">Rules are combined using "or".</span></span>|

## <a name="relationships"></a><span data-ttu-id="14391-114">Relações</span><span class="sxs-lookup"><span data-stu-id="14391-114">Relationships</span></span>
<span data-ttu-id="14391-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14391-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14391-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14391-116">JSON representation</span></span>
<span data-ttu-id="14391-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14391-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringSettings",
  "monitoringRules": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
    }
  ]
}
```

