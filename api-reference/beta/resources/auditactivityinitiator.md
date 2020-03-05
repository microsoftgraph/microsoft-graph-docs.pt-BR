---
title: tipo de recurso auditActivityInitiator
description: Identity o objeto Resource que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2d74b9d268bf61ee191fb2a8b35368b08dd5650d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508091"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="0280a-104">tipo de recurso auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="0280a-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="0280a-105">Namespace: Microsoft. Graph Identity o objeto Resource que inicia a atividade.</span><span class="sxs-lookup"><span data-stu-id="0280a-105">Namespace: microsoft.graph Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="0280a-106">O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)</span><span class="sxs-lookup"><span data-stu-id="0280a-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="0280a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0280a-107">Properties</span></span>
| <span data-ttu-id="0280a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0280a-108">Property</span></span>     | <span data-ttu-id="0280a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0280a-109">Type</span></span>   |<span data-ttu-id="0280a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0280a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0280a-111">aplicativo</span><span class="sxs-lookup"><span data-stu-id="0280a-111">app</span></span>|[<span data-ttu-id="0280a-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="0280a-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="0280a-113">Se o recurso que inicia a atividade for um aplicativo, essa propriedade indica todas as informações relacionadas ao aplicativo, como appId, Name, servicePrincipalName, Name.</span><span class="sxs-lookup"><span data-stu-id="0280a-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="0280a-114">user</span><span class="sxs-lookup"><span data-stu-id="0280a-114">user</span></span>|[<span data-ttu-id="0280a-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="0280a-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="0280a-116">Se o recurso que inicia a atividade for um usuário, essa propriedade indicará todas as informações relacionadas ao usuário, como userId, Name, UserPrinicpalName.</span><span class="sxs-lookup"><span data-stu-id="0280a-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0280a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0280a-117">JSON representation</span></span>

<span data-ttu-id="0280a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0280a-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
