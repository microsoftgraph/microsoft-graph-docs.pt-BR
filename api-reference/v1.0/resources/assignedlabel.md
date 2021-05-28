---
title: Tipo de recurso assignedLabel
description: Representa um rótulo de sensibilidade atribuído a um Microsoft 365 grupo.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: ea71e19388e8d9aa1bdf7f85c85ba6a85249233a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680462"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="db37e-103">Tipo de recurso assignedLabel</span><span class="sxs-lookup"><span data-stu-id="db37e-103">assignedLabel resource type</span></span>

<span data-ttu-id="db37e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db37e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db37e-105">Representa um rótulo de sensibilidade atribuído a um Microsoft 365 grupo.</span><span class="sxs-lookup"><span data-stu-id="db37e-105">Represents a sensitivity label assigned to an Microsoft 365 group.</span></span> <span data-ttu-id="db37e-106">Os rótulos de confidencialidade permitem que os administradores imigam configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral).</span><span class="sxs-lookup"><span data-stu-id="db37e-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="db37e-107">Os rótulos de sensibilidade são publicados pelos administradores no centro de conformidade Microsoft 365 segurança & como parte dos recursos da Proteção de Informações da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="db37e-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="db37e-108">Para obter mais informações sobre rótulos de sensibilidade, consulte [Visão geral dos rótulos de sensibilidade.](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="db37e-108">For more information about sensitivity labels, see [Sensitivity labels overview](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span></span>

## <a name="properties"></a><span data-ttu-id="db37e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db37e-109">Properties</span></span>
| <span data-ttu-id="db37e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db37e-110">Property</span></span>     | <span data-ttu-id="db37e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="db37e-111">Type</span></span>   |<span data-ttu-id="db37e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="db37e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db37e-113">labelId</span><span class="sxs-lookup"><span data-stu-id="db37e-113">labelId</span></span>|<span data-ttu-id="db37e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db37e-114">String</span></span>|<span data-ttu-id="db37e-115">O identificador exclusivo do rótulo.</span><span class="sxs-lookup"><span data-stu-id="db37e-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="db37e-116">displayName</span><span class="sxs-lookup"><span data-stu-id="db37e-116">displayName</span></span>|<span data-ttu-id="db37e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db37e-117">String</span></span>|<span data-ttu-id="db37e-118">O nome de exibição do rótulo.</span><span class="sxs-lookup"><span data-stu-id="db37e-118">The display name of the label.</span></span> <span data-ttu-id="db37e-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db37e-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db37e-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db37e-120">JSON representation</span></span>

<span data-ttu-id="db37e-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db37e-121">Here is a JSON representation of the resource.</span></span>

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