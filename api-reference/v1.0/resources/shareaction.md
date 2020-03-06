---
author: daspek
ms.author: dspektor
title: tipo de recurso shareaction
description: O objeto shareaction fornece informações sobre quem um item foi compartilhado em uma ação de compartilhamento.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f8b4870ec82a2f264d6f67cdd02cd22c9747e51e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533733"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="c864b-103">tipo de recurso shareaction</span><span class="sxs-lookup"><span data-stu-id="c864b-103">shareAction resource type</span></span>

<span data-ttu-id="c864b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c864b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c864b-105">O recurso **shareaction** fornece informações sobre uma [atividade][activity] que compartilhou um item.</span><span class="sxs-lookup"><span data-stu-id="c864b-105">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="c864b-106">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="c864b-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="c864b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c864b-107">Properties</span></span>

| <span data-ttu-id="c864b-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c864b-108">Property name</span></span> | <span data-ttu-id="c864b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c864b-109">Type</span></span>                       | <span data-ttu-id="c864b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c864b-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="c864b-111">destinatários</span><span class="sxs-lookup"><span data-stu-id="c864b-111">recipients</span></span>    | <span data-ttu-id="c864b-112">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c864b-112">[identitySet][] collection</span></span> | <span data-ttu-id="c864b-113">As identidades com as quais o item foi compartilhado nesta ação.</span><span class="sxs-lookup"><span data-stu-id="c864b-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="c864b-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c864b-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->
