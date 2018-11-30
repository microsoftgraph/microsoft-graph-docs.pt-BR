---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
ms.openlocfilehash: be873ba2b5f9bc1fdd387407c1036435dc6f1fc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036260"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="ec224-102">Tipo de recurso MentionAction</span><span class="sxs-lookup"><span data-stu-id="ec224-102">MentionAction resource type</span></span>

> <span data-ttu-id="ec224-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec224-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec224-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec224-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec224-105">O recurso **MentionAction** fornece informações sobre um [atividade][] que mencionou pessoas.</span><span class="sxs-lookup"><span data-stu-id="ec224-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[atividade]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="ec224-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec224-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="ec224-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec224-108">Properties</span></span>

| <span data-ttu-id="ec224-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ec224-109">Property name</span></span> | <span data-ttu-id="ec224-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec224-110">Type</span></span>                       | <span data-ttu-id="ec224-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec224-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="ec224-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="ec224-112">mentionees</span></span>    | <span data-ttu-id="ec224-113">Coleção [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ec224-113">[identitySet][] collection</span></span> | <span data-ttu-id="ec224-114">As identidades dos usuários mencionados nesta ação.</span><span class="sxs-lookup"><span data-stu-id="ec224-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="ec224-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="ec224-116">Remarks</span></span>

<span data-ttu-id="ec224-117">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="ec224-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
