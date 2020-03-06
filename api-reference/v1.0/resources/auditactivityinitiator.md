---
title: tipo de recurso auditActivityInitiator
description: Identifica o objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo).
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0ed2a68d3e3fa07edb5b5b2ce0d969287ba9a7a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532046"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="6fa7d-104">tipo de recurso auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="6fa7d-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="6fa7d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fa7d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fa7d-106">Identity o objeto Resource que inicia a atividade.</span><span class="sxs-lookup"><span data-stu-id="6fa7d-106">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="6fa7d-107">O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado um aplicativo).</span><span class="sxs-lookup"><span data-stu-id="6fa7d-107">The initiator can be a user, an app, or a system (which is considered an app).</span></span>

## <a name="properties"></a><span data-ttu-id="6fa7d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fa7d-108">Properties</span></span>

| <span data-ttu-id="6fa7d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fa7d-109">Property</span></span>     | <span data-ttu-id="6fa7d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fa7d-110">Type</span></span>   |<span data-ttu-id="6fa7d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa7d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fa7d-112">aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fa7d-112">app</span></span>|[<span data-ttu-id="6fa7d-113">appIdentity</span><span class="sxs-lookup"><span data-stu-id="6fa7d-113">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="6fa7d-114">Se o recurso que inicia a atividade for um aplicativo, essa propriedade indica todas as informações relacionadas ao aplicativo, como appId, Name, servicePrincipalName, Name.</span><span class="sxs-lookup"><span data-stu-id="6fa7d-114">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="6fa7d-115">user</span><span class="sxs-lookup"><span data-stu-id="6fa7d-115">user</span></span>|[<span data-ttu-id="6fa7d-116">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6fa7d-116">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="6fa7d-117">Se o recurso que inicia a atividade for um usuário, essa propriedade indicará todas as informações relacionadas ao usuário, como userId, Name, UserPrinicpalName.</span><span class="sxs-lookup"><span data-stu-id="6fa7d-117">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fa7d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fa7d-118">JSON representation</span></span>

<span data-ttu-id="6fa7d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fa7d-119">Here is a JSON representation of the resource.</span></span>

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
