---
title: tipo de recurso conditionalAccessApplications
description: Representa os aplicativos e as ações do usuário incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba904fec35830bef6cc5a74daa1c4938bd99d250
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269907"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="2d139-103">tipo de recurso conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="2d139-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="2d139-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d139-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d139-105">Representa os aplicativos e as ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="2d139-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="2d139-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d139-106">Properties</span></span>

| <span data-ttu-id="2d139-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d139-107">Property</span></span> | <span data-ttu-id="2d139-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d139-108">Type</span></span> | <span data-ttu-id="2d139-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d139-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="2d139-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="2d139-110">includeApplications</span></span> | <span data-ttu-id="2d139-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d139-111">String collection</span></span> | <span data-ttu-id="2d139-112">A lista de IDs de aplicativo à qual a política se aplica, a menos que explicitamente excluída (em excludeApplications).</span><span class="sxs-lookup"><span data-stu-id="2d139-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="2d139-113">Também pode ser definido como `All` .</span><span class="sxs-lookup"><span data-stu-id="2d139-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="2d139-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="2d139-114">excludeApplications</span></span> | <span data-ttu-id="2d139-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d139-115">String collection</span></span> | <span data-ttu-id="2d139-116">A lista de IDs de aplicativo explicitamente excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="2d139-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="2d139-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="2d139-117">includeUserActions</span></span> | <span data-ttu-id="2d139-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d139-118">String collection</span></span> | <span data-ttu-id="2d139-119">Ações do usuário a serem incluídas.</span><span class="sxs-lookup"><span data-stu-id="2d139-119">User actions to include.</span></span> <span data-ttu-id="2d139-120">Os valores com suporte são `urn:user:registersecurityinfo` e `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="2d139-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |

## <a name="relationships"></a><span data-ttu-id="2d139-121">Relações</span><span class="sxs-lookup"><span data-stu-id="2d139-121">Relationships</span></span>

<span data-ttu-id="2d139-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d139-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d139-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d139-123">JSON representation</span></span>

<span data-ttu-id="2d139-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d139-124">The following is a JSON representation of the resource.</span></span>

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

