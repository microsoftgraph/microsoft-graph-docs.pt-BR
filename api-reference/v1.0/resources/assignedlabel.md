---
title: Tipo de recurso assignedLabel
description: Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: fa95223aadc4a0b065a3227967a27c8b66b3bff1
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761518"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="9c6d0-103">Tipo de recurso assignedLabel</span><span class="sxs-lookup"><span data-stu-id="9c6d0-103">assignedLabel resource type</span></span>

<span data-ttu-id="9c6d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c6d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c6d0-105">Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-105">Represents a sensitivity label assigned to an Microsoft 365 group.</span></span> <span data-ttu-id="9c6d0-106">Os rótulos de confidencialidade permitem que os administradores imigam configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral).</span><span class="sxs-lookup"><span data-stu-id="9c6d0-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="9c6d0-107">Os rótulos de sensibilidade são publicados pelos administradores no Centro de Conformidade e Segurança do Microsoft 365 & como parte dos recursos de Proteção de Informações da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="9c6d0-108">Para obter mais informações sobre rótulos de sensibilidade, consulte [Visão geral dos rótulos de sensibilidade.](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="9c6d0-108">For more information about sensitivity labels, see [Sensitivity labels overview](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span></span>

## <a name="properties"></a><span data-ttu-id="9c6d0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c6d0-109">Properties</span></span>
| <span data-ttu-id="9c6d0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c6d0-110">Property</span></span>     | <span data-ttu-id="9c6d0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c6d0-111">Type</span></span>   |<span data-ttu-id="9c6d0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c6d0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c6d0-113">labelId</span><span class="sxs-lookup"><span data-stu-id="9c6d0-113">labelId</span></span>|<span data-ttu-id="9c6d0-114">String</span><span class="sxs-lookup"><span data-stu-id="9c6d0-114">String</span></span>|<span data-ttu-id="9c6d0-115">O identificador exclusivo do rótulo.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="9c6d0-116">displayName</span><span class="sxs-lookup"><span data-stu-id="9c6d0-116">displayName</span></span>|<span data-ttu-id="9c6d0-117">String</span><span class="sxs-lookup"><span data-stu-id="9c6d0-117">String</span></span>|<span data-ttu-id="9c6d0-118">O nome de exibição do rótulo.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-118">The display name of the label.</span></span> <span data-ttu-id="9c6d0-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c6d0-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c6d0-120">JSON representation</span></span>

<span data-ttu-id="9c6d0-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c6d0-121">Here is a JSON representation of the resource.</span></span>

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