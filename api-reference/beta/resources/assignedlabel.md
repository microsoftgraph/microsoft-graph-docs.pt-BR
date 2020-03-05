---
title: tipo de recurso assignedLabel
description: Representa um rótulo de confidencialidade atribuído a um grupo do Office 365. Os rótulos de confidencialidade permitem que os administradores imponham configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como confidencial, altamente confidencial ou geral).
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 4f4f1fd854885668160b46f2b1ee9396dcf954fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508216"
---
# <a name="assignedlabel-resource-type"></a><span data-ttu-id="54c4c-104">tipo de recurso assignedLabel</span><span class="sxs-lookup"><span data-stu-id="54c4c-104">assignedLabel resource type</span></span>

<span data-ttu-id="54c4c-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="54c4c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54c4c-106">Representa um rótulo de confidencialidade atribuído a um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="54c4c-106">Represents a sensitivity label assigned to an Office 365 group.</span></span> <span data-ttu-id="54c4c-107">Os rótulos de confidencialidade permitem que os administradores imponham configurações de grupo específicas em um grupo atribuindo uma classificação ao grupo (como confidencial, altamente confidencial ou geral).</span><span class="sxs-lookup"><span data-stu-id="54c4c-107">Sensitivity labels allow administrators to enforce specific group settings on a group by assigning a classification to the group (such as Confidential, Highly Confidential or General).</span></span> <span data-ttu-id="54c4c-108">Os rótulos de confidencialidade são publicados por administradores no centro de conformidade & segurança da Microsoft 365 como parte dos recursos de proteção de informações da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="54c4c-108">Sensitivity labels are published by administrators in Microsoft 365 Security & Compliance Center as part of Microsoft Information Protection capabilities.</span></span> <span data-ttu-id="54c4c-109">Para obter mais informações sobre rótulos de sensibilidade, consulte [visão geral dos rótulos de sensibilidade](/Office365/SecurityCompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="54c4c-109">For more information about sensitivity labels, see [Sensitivity labels overview](/Office365/SecurityCompliance/sensitivity-labels).</span></span>

## <a name="properties"></a><span data-ttu-id="54c4c-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54c4c-110">Properties</span></span>
| <span data-ttu-id="54c4c-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54c4c-111">Property</span></span>     | <span data-ttu-id="54c4c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="54c4c-112">Type</span></span>   |<span data-ttu-id="54c4c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="54c4c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54c4c-114">labelID</span><span class="sxs-lookup"><span data-stu-id="54c4c-114">labelId</span></span>|<span data-ttu-id="54c4c-115">String</span><span class="sxs-lookup"><span data-stu-id="54c4c-115">String</span></span>|<span data-ttu-id="54c4c-116">O identificador exclusivo do rótulo.</span><span class="sxs-lookup"><span data-stu-id="54c4c-116">The unique identifier of the label.</span></span>|
|<span data-ttu-id="54c4c-117">displayName</span><span class="sxs-lookup"><span data-stu-id="54c4c-117">displayName</span></span>|<span data-ttu-id="54c4c-118">String</span><span class="sxs-lookup"><span data-stu-id="54c4c-118">String</span></span>|<span data-ttu-id="54c4c-119">O nome de exibição do rótulo.</span><span class="sxs-lookup"><span data-stu-id="54c4c-119">The display name of the label.</span></span> <span data-ttu-id="54c4c-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54c4c-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54c4c-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54c4c-121">JSON representation</span></span>

<span data-ttu-id="54c4c-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54c4c-122">Here is a JSON representation of the resource.</span></span>

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
