---
title: Tipo de recurso assignedLabel
description: Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365.
localization_priority: Normal
author: jpettere
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 9602e10dda5d558110c55f1fb4ee166e53187989
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720890"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="7ea31-103">Tipo de recurso assignedLabel</span><span class="sxs-lookup"><span data-stu-id="7ea31-103">assignedLabel resource type</span></span>

<span data-ttu-id="7ea31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ea31-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ea31-105">Representa um rótulo de sensibilidade atribuído a um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7ea31-105">Represents a sensitivity label assigned to an Microsoft 365 group.</span></span> <span data-ttu-id="7ea31-106">Os rótulos de confidencialidade permitem que os administradores imigam configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como Confidencial, Altamente Confidencial ou Geral).</span><span class="sxs-lookup"><span data-stu-id="7ea31-106">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="7ea31-107">Os rótulos de sensibilidade são publicados pelos administradores no Centro de Conformidade e Segurança do Microsoft 365 & como parte dos recursos de Proteção de Informações da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7ea31-107">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="7ea31-108">Para obter mais informações sobre rótulos de sensibilidade, consulte [Visão geral dos rótulos de sensibilidade.](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="7ea31-108">For more information about sensitivity labels, see [Sensitivity labels overview](/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).</span></span>

## <a name="properties"></a><span data-ttu-id="7ea31-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ea31-109">Properties</span></span>
| <span data-ttu-id="7ea31-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ea31-110">Property</span></span>     | <span data-ttu-id="7ea31-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ea31-111">Type</span></span>   |<span data-ttu-id="7ea31-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ea31-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ea31-113">labelId</span><span class="sxs-lookup"><span data-stu-id="7ea31-113">labelId</span></span>|<span data-ttu-id="7ea31-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ea31-114">String</span></span>|<span data-ttu-id="7ea31-115">O identificador exclusivo do rótulo.</span><span class="sxs-lookup"><span data-stu-id="7ea31-115">The unique identifier of the label.</span></span>|
|<span data-ttu-id="7ea31-116">displayName</span><span class="sxs-lookup"><span data-stu-id="7ea31-116">displayName</span></span>|<span data-ttu-id="7ea31-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ea31-117">String</span></span>|<span data-ttu-id="7ea31-118">O nome de exibição do rótulo.</span><span class="sxs-lookup"><span data-stu-id="7ea31-118">The display name of the label.</span></span> <span data-ttu-id="7ea31-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ea31-119">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ea31-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ea31-120">JSON representation</span></span>

<span data-ttu-id="7ea31-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ea31-121">Here is a JSON representation of the resource.</span></span>

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