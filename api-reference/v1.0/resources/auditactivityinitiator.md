---
title: tipo de recurso auditActivityInitiator
description: Identifica o objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo).
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5de4cc65379a3386137c7da79a10c5492dd1427
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629345"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="00755-104">tipo de recurso auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="00755-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="00755-105">Identity o objeto Resource que inicia a atividade.</span><span class="sxs-lookup"><span data-stu-id="00755-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="00755-106">O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado um aplicativo).</span><span class="sxs-lookup"><span data-stu-id="00755-106">The initiator can be a user, an app, or a system (which is considered an app).</span></span>

## <a name="properties"></a><span data-ttu-id="00755-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00755-107">Properties</span></span>

| <span data-ttu-id="00755-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00755-108">Property</span></span>     | <span data-ttu-id="00755-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="00755-109">Type</span></span>   |<span data-ttu-id="00755-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="00755-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00755-111">aplicativo</span><span class="sxs-lookup"><span data-stu-id="00755-111">app</span></span>|[<span data-ttu-id="00755-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="00755-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="00755-113">Se o recurso que inicia a atividade for um aplicativo, essa propriedade indica todas as informações relacionadas ao aplicativo, como appId, Name, servicePrincipalName, Name.</span><span class="sxs-lookup"><span data-stu-id="00755-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="00755-114">user</span><span class="sxs-lookup"><span data-stu-id="00755-114">user</span></span>|[<span data-ttu-id="00755-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="00755-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="00755-116">Se o recurso que inicia a atividade for um usuário, essa propriedade indicará todas as informações relacionadas ao usuário, como userId, Name, UserPrinicpalName.</span><span class="sxs-lookup"><span data-stu-id="00755-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00755-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00755-117">JSON representation</span></span>

<span data-ttu-id="00755-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00755-118">Here is a JSON representation of the resource.</span></span>

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
