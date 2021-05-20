---
title: Tipo de recurso conditionalAccessApplications
description: Representa aplicativos e ações do usuário incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d688b529e32390c2330cf8cb3558994c3e752a25
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547680"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="e21af-103">Tipo de recurso conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="e21af-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="e21af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e21af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e21af-105">Representa os aplicativos e as ações do usuário incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="e21af-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="e21af-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e21af-106">Properties</span></span>

| <span data-ttu-id="e21af-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e21af-107">Property</span></span> | <span data-ttu-id="e21af-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e21af-108">Type</span></span> | <span data-ttu-id="e21af-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e21af-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="e21af-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="e21af-110">includeApplications</span></span> | <span data-ttu-id="e21af-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e21af-111">String collection</span></span> | <span data-ttu-id="e21af-112">A lista de IDs de aplicativo a que a política se aplica, a menos que seja explicitamente excluída (em excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="e21af-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="e21af-113">Também pode ser definido como `All` .</span><span class="sxs-lookup"><span data-stu-id="e21af-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="e21af-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="e21af-114">excludeApplications</span></span> | <span data-ttu-id="e21af-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e21af-115">String collection</span></span> | <span data-ttu-id="e21af-116">A lista de IDs de aplicativos excluídas explicitamente da política.</span><span class="sxs-lookup"><span data-stu-id="e21af-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="e21af-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="e21af-117">includeUserActions</span></span> | <span data-ttu-id="e21af-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e21af-118">String collection</span></span> | <span data-ttu-id="e21af-119">Ações do usuário a incluir.</span><span class="sxs-lookup"><span data-stu-id="e21af-119">User actions to include.</span></span> <span data-ttu-id="e21af-120">Os valores com suporte `urn:user:registersecurityinfo` são e `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="e21af-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |
| <span data-ttu-id="e21af-121">includeAuthenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="e21af-121">includeAuthenticationContextClassReferences</span></span> | <span data-ttu-id="e21af-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e21af-122">String collection</span></span> | <span data-ttu-id="e21af-123">As referências de classe de contexto de autenticação incluem.</span><span class="sxs-lookup"><span data-stu-id="e21af-123">Authentication context class references include.</span></span> <span data-ttu-id="e21af-124">Os valores suportados são `c1` através `c25` de .</span><span class="sxs-lookup"><span data-stu-id="e21af-124">Supported values are `c1` through `c25`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e21af-125">Relações</span><span class="sxs-lookup"><span data-stu-id="e21af-125">Relationships</span></span>

<span data-ttu-id="e21af-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e21af-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e21af-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e21af-127">JSON representation</span></span>

<span data-ttu-id="e21af-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e21af-128">The following is a JSON representation of the resource.</span></span>

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

