---
title: Tipo de recurso win32LobAppRule
description: Um tipo complexo básico para armazenar os dados de regra de detecção ou requisito para um aplicativo LOB win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1494aa6089bac73ae14612804009237bb9a5b2fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758957"
---
# <a name="win32lobapprule-resource-type"></a><span data-ttu-id="e4630-103">Tipo de recurso win32LobAppRule</span><span class="sxs-lookup"><span data-stu-id="e4630-103">win32LobAppRule resource type</span></span>

<span data-ttu-id="e4630-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4630-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4630-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4630-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4630-106">Um tipo complexo básico para armazenar os dados de regra de detecção ou requisito para um aplicativo LOB win32.</span><span class="sxs-lookup"><span data-stu-id="e4630-106">A base complex type to store the detection or requirement rule data for a Win32 LOB app.</span></span>

## <a name="properties"></a><span data-ttu-id="e4630-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4630-107">Properties</span></span>
|<span data-ttu-id="e4630-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4630-108">Property</span></span>|<span data-ttu-id="e4630-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4630-109">Type</span></span>|<span data-ttu-id="e4630-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4630-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4630-111">ruleType</span><span class="sxs-lookup"><span data-stu-id="e4630-111">ruleType</span></span>|[<span data-ttu-id="e4630-112">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="e4630-112">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="e4630-113">O tipo de regra que indica a finalidade da regra.</span><span class="sxs-lookup"><span data-stu-id="e4630-113">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="e4630-114">Os valores possíveis são: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="e4630-114">Possible values are: `detection`, `requirement`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4630-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e4630-115">Relationships</span></span>
<span data-ttu-id="e4630-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e4630-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4630-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4630-117">JSON Representation</span></span>
<span data-ttu-id="e4630-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4630-118">Here is a JSON representation of the resource.</span></span>
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




