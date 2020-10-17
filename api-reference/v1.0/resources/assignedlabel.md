---
title: tipo de recurso assignedLabel
description: Representa um rótulo de confidencialidade atribuído a um grupo do Microsoft 365.
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 923b616c024a240407161b909baf22ac73d590cc
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581950"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="36ecd-103">tipo de recurso assignedLabel</span><span class="sxs-lookup"><span data-stu-id="36ecd-103">assignedLabel resource type</span></span>

<span data-ttu-id="36ecd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36ecd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36ecd-105">Representa um rótulo de confidencialidade atribuído a um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="36ecd-105">Represents a sensitivity label assigned to an Microsoft 365 group.</span></span> <span data-ttu-id="36ecd-106">Os rótulos de confidencialidade permitem que os administradores imponham configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como confidencial, altamente confidencial ou geral).</span><span class="sxs-lookup"><span data-stu-id="36ecd-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="36ecd-107">Os rótulos de confidencialidade são publicados por administradores no centro de conformidade & segurança da Microsoft 365 como parte dos recursos de proteção de informações da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="36ecd-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="36ecd-108">Para obter mais informações sobre rótulos de sensibilidade, consulte [visão geral dos rótulos de sensibilidade](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="36ecd-108">For more information about sensitivity labels, see [Sensitivity labels overview](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span></span>

## <a name="properties"></a><span data-ttu-id="36ecd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36ecd-109">Properties</span></span>
| <span data-ttu-id="36ecd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36ecd-110">Property</span></span>     | <span data-ttu-id="36ecd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="36ecd-111">Type</span></span>   |<span data-ttu-id="36ecd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="36ecd-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36ecd-113">labelID</span><span class="sxs-lookup"><span data-stu-id="36ecd-113">labelId</span></span>|<span data-ttu-id="36ecd-114">String</span><span class="sxs-lookup"><span data-stu-id="36ecd-114">String</span></span>|<span data-ttu-id="36ecd-115">O identificador exclusivo do rótulo.</span><span class="sxs-lookup"><span data-stu-id="36ecd-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="36ecd-116">displayName</span><span class="sxs-lookup"><span data-stu-id="36ecd-116">displayName</span></span>|<span data-ttu-id="36ecd-117">String</span><span class="sxs-lookup"><span data-stu-id="36ecd-117">String</span></span>|<span data-ttu-id="36ecd-118">O nome de exibição do rótulo.</span><span class="sxs-lookup"><span data-stu-id="36ecd-118">The display name of the label.</span></span> <span data-ttu-id="36ecd-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36ecd-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36ecd-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36ecd-120">JSON representation</span></span>

<span data-ttu-id="36ecd-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36ecd-121">Here is a JSON representation of the resource.</span></span>

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