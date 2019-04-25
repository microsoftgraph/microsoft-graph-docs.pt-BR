---
title: tipo de recurso plannerUserIds
description: O recurso **plannerUserIds** representa a lista de IDs de usuários com as quais um plano é compartilhado. Este é um tipo aberto. Se estiver aproveitando os grupos do Office 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano do grupo. Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 33a1d6472f4c146d0875ec35fdee920652b7de39
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576007"
---
# <a name="planneruserids-resource-type"></a><span data-ttu-id="db73e-106">tipo de recurso plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="db73e-106">plannerUserIds resource type</span></span>

<span data-ttu-id="db73e-107">O recurso **plannerUserIds** representa a lista de IDs de usuários com as quais um [plano](plannerplan.md) é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="db73e-107">The **plannerUserIds** resource represents the list of users ids that a [plan](plannerplan.md) is shared with.</span></span> <span data-ttu-id="db73e-108">Este é um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="db73e-108">This is an Open Type.</span></span> <span data-ttu-id="db73e-109">Se estiver aproveitando os grupos do Office 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) .</span><span class="sxs-lookup"><span data-stu-id="db73e-109">If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="db73e-110">Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="db73e-110">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span>


## <a name="properties"></a><span data-ttu-id="db73e-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db73e-111">Properties</span></span>
<span data-ttu-id="db73e-112">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="db73e-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="db73e-113">Nesse caso, o cliente deve fornecer IDs de usuário como propriedades com seus valores como `true` Boolean.</span><span class="sxs-lookup"><span data-stu-id="db73e-113">In this case, the client should provide user ids as properties with their values being the `true` boolean.</span></span> <span data-ttu-id="db73e-114">Quando as IDs de usuário não são mais compartilhadas, as propriedades são removidas automaticamente `false` definindo seus valores para o Boolean.</span><span class="sxs-lookup"><span data-stu-id="db73e-114">When user ids are no longer shared with, properties are automatically removed by setting their values to the `false` boolean.</span></span>


## <a name="json-representation"></a><span data-ttu-id="db73e-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db73e-115">JSON representation</span></span>

<span data-ttu-id="db73e-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="db73e-116">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="db73e-117">Como</span><span class="sxs-lookup"><span data-stu-id="db73e-117">// Example</span></span>
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
