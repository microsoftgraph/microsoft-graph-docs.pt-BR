---
author: daspek
title: Tipo de recurso shareAction
description: O objeto shareAction fornece informações sobre com quem um item foi compartilhado em uma ação de compartilhamento.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 81292f302667123c0d22f78b655e4ef555329e52
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238887"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="63d28-103">Tipo de recurso shareAction</span><span class="sxs-lookup"><span data-stu-id="63d28-103">shareAction resource type</span></span>

<span data-ttu-id="63d28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63d28-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63d28-105">O **recurso shareAction** fornece informações sobre uma [atividade que][activity] compartilhou um item.</span><span class="sxs-lookup"><span data-stu-id="63d28-105">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="63d28-106">**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="63d28-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="63d28-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63d28-107">Properties</span></span>

| <span data-ttu-id="63d28-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="63d28-108">Property name</span></span> | <span data-ttu-id="63d28-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="63d28-109">Type</span></span>                       | <span data-ttu-id="63d28-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="63d28-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="63d28-111">destinatários</span><span class="sxs-lookup"><span data-stu-id="63d28-111">recipients</span></span>    | <span data-ttu-id="63d28-112">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="63d28-112">[identitySet][] collection</span></span> | <span data-ttu-id="63d28-113">As identidades com as quais o item foi compartilhado nesta ação.</span><span class="sxs-lookup"><span data-stu-id="63d28-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="63d28-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63d28-115">JSON representation</span></span>

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

