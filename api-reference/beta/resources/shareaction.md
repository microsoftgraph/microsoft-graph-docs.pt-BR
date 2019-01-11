---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
ms.openlocfilehash: 16bc590fcfe14f9ce7f6f1bbe38492225cce099c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828655"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="4c93e-102">Tipo de recurso ShareAction</span><span class="sxs-lookup"><span data-stu-id="4c93e-102">ShareAction resource type</span></span>

> <span data-ttu-id="4c93e-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4c93e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c93e-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4c93e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c93e-105">O recurso **ShareAction** fornece informações sobre uma [activity][activity] que compartilhou um item.</span><span class="sxs-lookup"><span data-stu-id="4c93e-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="4c93e-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c93e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4c93e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c93e-107">Properties</span></span>

| <span data-ttu-id="4c93e-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4c93e-108">Property name</span></span> | <span data-ttu-id="4c93e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c93e-109">Type</span></span>                       | <span data-ttu-id="4c93e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c93e-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="4c93e-111">recipients</span><span class="sxs-lookup"><span data-stu-id="4c93e-111">recipients</span></span>    | <span data-ttu-id="4c93e-112">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4c93e-112">[identitySet][] collection</span></span> | <span data-ttu-id="4c93e-113">As identidades com as quais o item foi compartilhado nesta ação.</span><span class="sxs-lookup"><span data-stu-id="4c93e-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="4c93e-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="4c93e-115">Remarks</span></span>

<span data-ttu-id="4c93e-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="4c93e-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction"
} -->
