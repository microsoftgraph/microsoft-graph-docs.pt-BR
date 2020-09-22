---
title: tipo de recurso win32LobAppRule
description: Um tipo base complexo para armazenar os dados de regra de detecção ou requisito para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 086805088c5b36cb3ab61f9117aa337f913f0386
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036687"
---
# <a name="win32lobapprule-resource-type"></a><span data-ttu-id="ec942-103">tipo de recurso win32LobAppRule</span><span class="sxs-lookup"><span data-stu-id="ec942-103">win32LobAppRule resource type</span></span>

<span data-ttu-id="ec942-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec942-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec942-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec942-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec942-106">Um tipo base complexo para armazenar os dados de regra de detecção ou requisito para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="ec942-106">A base complex type to store the detection or requirement rule data for a Win32 LOB app.</span></span>

## <a name="properties"></a><span data-ttu-id="ec942-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec942-107">Properties</span></span>
|<span data-ttu-id="ec942-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec942-108">Property</span></span>|<span data-ttu-id="ec942-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec942-109">Type</span></span>|<span data-ttu-id="ec942-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec942-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec942-111">ruleType</span><span class="sxs-lookup"><span data-stu-id="ec942-111">ruleType</span></span>|[<span data-ttu-id="ec942-112">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="ec942-112">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="ec942-113">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="ec942-113">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="ec942-114">Os valores possíveis são: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="ec942-114">Possible values are: `detection`, `requirement`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec942-115">Relações</span><span class="sxs-lookup"><span data-stu-id="ec942-115">Relationships</span></span>
<span data-ttu-id="ec942-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec942-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec942-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec942-117">JSON Representation</span></span>
<span data-ttu-id="ec942-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec942-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRule",
  "ruleType": "String"
}
```





