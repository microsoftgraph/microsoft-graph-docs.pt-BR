---
title: tipo de recurso plannerUserIds
description: O recurso **plannerUserIds** representa a lista de IDs de usuários com as quais um plano é compartilhado. Este é um tipo aberto. Se você estiver aproveitando os grupos do Microsoft 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano do grupo. Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e8e63a757e659ea6d2baf709019d17d353279493
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811291"
---
# <a name="planneruserids-resource-type"></a><span data-ttu-id="b1836-106">tipo de recurso plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="b1836-106">plannerUserIds resource type</span></span>

<span data-ttu-id="b1836-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1836-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1836-108">O recurso **plannerUserIds** representa a lista de IDs de usuários com as quais um [plano](plannerplan.md) é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b1836-108">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with.</span></span> <span data-ttu-id="b1836-109">Este é um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="b1836-109">This is an Open Type.</span></span> <span data-ttu-id="b1836-110">Se você estiver aproveitando os grupos do Microsoft 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) .</span><span class="sxs-lookup"><span data-stu-id="b1836-110">If you are leveraging Microsoft 365 groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="b1836-111">Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="b1836-111">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="b1836-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1836-112">Properties</span></span>
<span data-ttu-id="b1836-113">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b1836-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="b1836-114">Nesse caso, o cliente deve fornecer IDs de usuário como propriedades com seus valores como `true` Boolean.</span><span class="sxs-lookup"><span data-stu-id="b1836-114">In this case, the client should provide user ids as properties with their values being the `true` boolean.</span></span> <span data-ttu-id="b1836-115">Quando as IDs de usuário não são mais compartilhadas, as propriedades são removidas automaticamente definindo seus valores para o `false` Boolean.</span><span class="sxs-lookup"><span data-stu-id="b1836-115">When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1836-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1836-116">JSON representation</span></span>

<span data-ttu-id="b1836-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b1836-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

### <a name="example"></a><span data-ttu-id="b1836-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1836-118">Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
