---
title: Tipo de recurso assignedLabel
description: Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365. Os rótulos de confidencialidade permitem que os administradores imigam configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral).
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f22bfdd6cce307a83a90ada1da6a312994a3538e
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761244"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="985a5-104">Tipo de recurso assignedLabel</span><span class="sxs-lookup"><span data-stu-id="985a5-104">assignedLabel resource type</span></span>

<span data-ttu-id="985a5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="985a5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="985a5-106">Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="985a5-106">Represents a sensitivity label assigned to a Microsoft 365 group.</span></span> <span data-ttu-id="985a5-107">Os rótulos de confidencialidade permitem que os administradores imigam configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral).</span><span class="sxs-lookup"><span data-stu-id="985a5-107">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="985a5-108">Os rótulos de sensibilidade são publicados pelos administradores no Centro de Conformidade e Segurança do Microsoft 365 & como parte dos recursos de Proteção de Informações da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="985a5-108">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="985a5-109">Para obter mais informações sobre rótulos de sensibilidade, consulte [Visão geral dos rótulos de sensibilidade.](/Office365/SecurityCompliance/sensitivity-labels)</span><span class="sxs-lookup"><span data-stu-id="985a5-109">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="985a5-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="985a5-110">Properties</span></span>
| <span data-ttu-id="985a5-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="985a5-111">Property</span></span>     | <span data-ttu-id="985a5-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="985a5-112">Type</span></span>   |<span data-ttu-id="985a5-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="985a5-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="985a5-114">labelId</span><span class="sxs-lookup"><span data-stu-id="985a5-114">labelId</span></span>|<span data-ttu-id="985a5-115">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="985a5-115">String</span></span>|<span data-ttu-id="985a5-116">O identificador exclusivo do rótulo.</span><span class="sxs-lookup"><span data-stu-id="985a5-116">The unique identifier of the label.</span></span>|
|<span data-ttu-id="985a5-117">displayName</span><span class="sxs-lookup"><span data-stu-id="985a5-117">displayName</span></span>|<span data-ttu-id="985a5-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="985a5-118">String</span></span>|<span data-ttu-id="985a5-119">O nome de exibição do rótulo.</span><span class="sxs-lookup"><span data-stu-id="985a5-119">The display name of the label.</span></span> <span data-ttu-id="985a5-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="985a5-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="985a5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="985a5-121">JSON representation</span></span>

<span data-ttu-id="985a5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="985a5-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLabel"
}-->

```json
{
  "labelId": "String",
  "displayName": "String"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


