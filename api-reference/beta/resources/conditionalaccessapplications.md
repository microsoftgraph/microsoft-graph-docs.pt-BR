---
title: Tipo de recurso conditionalAccessApplications
description: Representa aplicativos e ações do usuário incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0a787a1c22209b502e4eed68790629e2e6e1b03b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137395"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="b12c5-103">Tipo de recurso conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="b12c5-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="b12c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b12c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b12c5-105">Representa os aplicativos e as ações do usuário incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="b12c5-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="b12c5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b12c5-106">Properties</span></span>

| <span data-ttu-id="b12c5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b12c5-107">Property</span></span> | <span data-ttu-id="b12c5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b12c5-108">Type</span></span> | <span data-ttu-id="b12c5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b12c5-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="b12c5-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="b12c5-110">includeApplications</span></span> | <span data-ttu-id="b12c5-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b12c5-111">String collection</span></span> | <span data-ttu-id="b12c5-112">A lista de IDs de aplicativos a que a política se aplica, a menos que explicitamente excluída (em excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="b12c5-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="b12c5-113">Também pode ser definido como `All` .</span><span class="sxs-lookup"><span data-stu-id="b12c5-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="b12c5-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="b12c5-114">excludeApplications</span></span> | <span data-ttu-id="b12c5-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b12c5-115">String collection</span></span> | <span data-ttu-id="b12c5-116">A lista de IDs de aplicativo explicitamente excluída da política.</span><span class="sxs-lookup"><span data-stu-id="b12c5-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="b12c5-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="b12c5-117">includeUserActions</span></span> | <span data-ttu-id="b12c5-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b12c5-118">String collection</span></span> | <span data-ttu-id="b12c5-119">Ações do usuário a incluir.</span><span class="sxs-lookup"><span data-stu-id="b12c5-119">User actions to include.</span></span> <span data-ttu-id="b12c5-120">Os valores com suporte `urn:user:registersecurityinfo` são e `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="b12c5-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |

## <a name="relationships"></a><span data-ttu-id="b12c5-121">Relações</span><span class="sxs-lookup"><span data-stu-id="b12c5-121">Relationships</span></span>

<span data-ttu-id="b12c5-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b12c5-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b12c5-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b12c5-123">JSON representation</span></span>

<span data-ttu-id="b12c5-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b12c5-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

