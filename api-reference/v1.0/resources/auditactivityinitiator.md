---
title: tipo de recurso auditActivityInitiator
description: Identifica o objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo).
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8d6d4d41698e6251c0f33a637dff9e667df7d092
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988510"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="d3b61-104">tipo de recurso auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="d3b61-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="d3b61-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3b61-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3b61-106">Identity o objeto Resource que inicia a atividade.</span><span class="sxs-lookup"><span data-stu-id="d3b61-106">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="d3b61-107">O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado um aplicativo).</span><span class="sxs-lookup"><span data-stu-id="d3b61-107">The initiator can be a user, an app, or a system (which is considered an app).</span></span>

## <a name="properties"></a><span data-ttu-id="d3b61-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3b61-108">Properties</span></span>

| <span data-ttu-id="d3b61-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3b61-109">Property</span></span>     | <span data-ttu-id="d3b61-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3b61-110">Type</span></span>   |<span data-ttu-id="d3b61-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3b61-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3b61-112">aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3b61-112">app</span></span>|[<span data-ttu-id="d3b61-113">appIdentity</span><span class="sxs-lookup"><span data-stu-id="d3b61-113">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="d3b61-114">Se o recurso que inicia a atividade for um aplicativo, essa propriedade indica todas as informações relacionadas ao aplicativo, como appId, Name, servicePrincipalName, Name.</span><span class="sxs-lookup"><span data-stu-id="d3b61-114">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="d3b61-115">user</span><span class="sxs-lookup"><span data-stu-id="d3b61-115">user</span></span>|[<span data-ttu-id="d3b61-116">userIdentity</span><span class="sxs-lookup"><span data-stu-id="d3b61-116">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="d3b61-117">Se o recurso que inicia a atividade for um usuário, essa propriedade indicará todas as informações relacionadas ao usuário, como userId, Name, UserPrinicpalName.</span><span class="sxs-lookup"><span data-stu-id="d3b61-117">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3b61-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3b61-118">JSON representation</span></span>

<span data-ttu-id="d3b61-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3b61-119">Here is a JSON representation of the resource.</span></span>

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

