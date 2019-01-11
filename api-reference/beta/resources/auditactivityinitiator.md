---
title: tipo de recurso de auditActivityInitiator
description: O objeto resource que inicia a atividade de identidade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)
localization_priority: Normal
ms.openlocfilehash: 14c92a4df42c3d8dbcd6836695df8d6caac3cf87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884606"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="d481b-104">tipo de recurso de auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="d481b-104">auditActivityInitiator resource type</span></span>
<span data-ttu-id="d481b-105">O objeto resource que inicia a atividade de identidade.</span><span class="sxs-lookup"><span data-stu-id="d481b-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="d481b-106">O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)</span><span class="sxs-lookup"><span data-stu-id="d481b-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="d481b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d481b-107">Properties</span></span>
| <span data-ttu-id="d481b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d481b-108">Property</span></span>     | <span data-ttu-id="d481b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d481b-109">Type</span></span>   |<span data-ttu-id="d481b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d481b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d481b-111">app</span><span class="sxs-lookup"><span data-stu-id="d481b-111">app</span></span>|[<span data-ttu-id="d481b-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="d481b-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="d481b-113">Se o recurso iniciando a atividade for um aplicativo, esta propriedade indica o aplicativo todas as informações como appId, relacionadas ao nome, servicePrincipalId, nome.</span><span class="sxs-lookup"><span data-stu-id="d481b-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="d481b-114">user</span><span class="sxs-lookup"><span data-stu-id="d481b-114">user</span></span>|[<span data-ttu-id="d481b-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="d481b-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="d481b-116">Se o recurso iniciando a atividade for um usuário, esta propriedade indica todos os usuários informações como userId, nome, UserPrinicpalName relacionadas.</span><span class="sxs-lookup"><span data-stu-id="d481b-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d481b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d481b-117">JSON representation</span></span>

<span data-ttu-id="d481b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d481b-118">Here is a JSON representation of the resource.</span></span>

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
