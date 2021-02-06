---
title: Tipo de recurso auditActivityInitiator
description: Identidade do objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: 71aa5e2bd09d66a2aea49058ceffea3e017eaf4d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131632"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="a9a0c-104">Tipo de recurso auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="a9a0c-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="a9a0c-105">Namespace: microsoft.graph Identity o objeto de recurso que inicia a atividade.</span><span class="sxs-lookup"><span data-stu-id="a9a0c-105">Namespace: microsoft.graph Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="a9a0c-106">O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo)</span><span class="sxs-lookup"><span data-stu-id="a9a0c-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="a9a0c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9a0c-107">Properties</span></span>
| <span data-ttu-id="a9a0c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9a0c-108">Property</span></span>     | <span data-ttu-id="a9a0c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9a0c-109">Type</span></span>   |<span data-ttu-id="a9a0c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9a0c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9a0c-111">aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9a0c-111">app</span></span>|[<span data-ttu-id="a9a0c-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="a9a0c-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="a9a0c-113">Se o recurso que inicia a atividade for um aplicativo, essa propriedade indicará todas as informações relacionadas ao aplicativo, como appId, Name, servicePrincipalId, Name.</span><span class="sxs-lookup"><span data-stu-id="a9a0c-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="a9a0c-114">user</span><span class="sxs-lookup"><span data-stu-id="a9a0c-114">user</span></span>|[<span data-ttu-id="a9a0c-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a9a0c-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="a9a0c-116">Se o recurso que inicia a atividade for um usuário, essa propriedade indicará todas as informações relacionadas ao usuário, como userId, Name, UserPrinicpalName.</span><span class="sxs-lookup"><span data-stu-id="a9a0c-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9a0c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9a0c-117">JSON representation</span></span>

<span data-ttu-id="a9a0c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9a0c-118">Here is a JSON representation of the resource.</span></span>

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


