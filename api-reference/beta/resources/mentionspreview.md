---
title: tipo de recurso de mentionsPreview
description: Representa informações sobre objetos mencionam em uma instância de recurso.
localization_priority: Normal
ms.openlocfilehash: 1534b7f0ef48a80d0faaaa09880b91cb270e8eca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826106"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="a2249-103">tipo de recurso de mentionsPreview</span><span class="sxs-lookup"><span data-stu-id="a2249-103">mentionsPreview resource type</span></span>

> <span data-ttu-id="a2249-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a2249-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2249-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a2249-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2249-106">Representa informações sobre objetos [mencionar](../resources/mention.md) em uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="a2249-106">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="a2249-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2249-107">Properties</span></span>
| <span data-ttu-id="a2249-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2249-108">Property</span></span>     | <span data-ttu-id="a2249-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2249-109">Type</span></span>   |<span data-ttu-id="a2249-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2249-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a2249-111">isMentioned</span><span class="sxs-lookup"><span data-stu-id="a2249-111">isMentioned</span></span> | <span data-ttu-id="a2249-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2249-112">Boolean</span></span> | <span data-ttu-id="a2249-113">True se o usuário entrou no mencionado na instância do recurso pai.</span><span class="sxs-lookup"><span data-stu-id="a2249-113">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="a2249-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2249-114">Read-only.</span></span> <span data-ttu-id="a2249-115">Suporta filtro.</span><span class="sxs-lookup"><span data-stu-id="a2249-115">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a2249-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2249-116">JSON representation</span></span>

<span data-ttu-id="a2249-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2249-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
