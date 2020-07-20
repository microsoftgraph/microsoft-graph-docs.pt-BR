---
title: tipo de recurso win32LobAppRule
description: Um tipo base complexo para armazenar os dados de regra de detecção ou requisito para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ffde7ad4549d3807602e7d02f088107e56541a44
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790289"
---
# <a name="win32lobapprule-resource-type"></a><span data-ttu-id="4d59b-103">tipo de recurso win32LobAppRule</span><span class="sxs-lookup"><span data-stu-id="4d59b-103">win32LobAppRule resource type</span></span>

<span data-ttu-id="4d59b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d59b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d59b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d59b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d59b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d59b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d59b-107">Um tipo base complexo para armazenar os dados de regra de detecção ou requisito para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="4d59b-107">A base complex type to store the detection or requirement rule data for a Win32 LOB app.</span></span>

## <a name="properties"></a><span data-ttu-id="4d59b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d59b-108">Properties</span></span>
|<span data-ttu-id="4d59b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d59b-109">Property</span></span>|<span data-ttu-id="4d59b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d59b-110">Type</span></span>|<span data-ttu-id="4d59b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d59b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d59b-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="4d59b-112">ruleType</span></span>|[<span data-ttu-id="4d59b-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="4d59b-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="4d59b-114">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="4d59b-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="4d59b-115">Os valores possíveis são: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="4d59b-115">Possible values are: `detection`, `requirement`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d59b-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4d59b-116">Relationships</span></span>
<span data-ttu-id="4d59b-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4d59b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d59b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d59b-118">JSON Representation</span></span>
<span data-ttu-id="4d59b-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d59b-119">Here is a JSON representation of the resource.</span></span>
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



