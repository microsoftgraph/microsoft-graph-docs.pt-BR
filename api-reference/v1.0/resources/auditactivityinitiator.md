---
title: Tipo de recurso auditActivityInitiator
description: Identifica o objeto de recurso que inicia a atividade. O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado como um aplicativo).
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fbc2fd2f6c93cac583fc1ec28375d8538d35b447
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135755"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="6f67e-104">Tipo de recurso auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="6f67e-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="6f67e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f67e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f67e-106">Identidade do objeto de recurso que inicia a atividade.</span><span class="sxs-lookup"><span data-stu-id="6f67e-106">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="6f67e-107">O iniciador pode ser um usuário, um aplicativo ou um sistema (que é considerado um aplicativo).</span><span class="sxs-lookup"><span data-stu-id="6f67e-107">The initiator can be a user, an app, or a system (which is considered an app).</span></span>

## <a name="properties"></a><span data-ttu-id="6f67e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f67e-108">Properties</span></span>

| <span data-ttu-id="6f67e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f67e-109">Property</span></span>     | <span data-ttu-id="6f67e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f67e-110">Type</span></span>   |<span data-ttu-id="6f67e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f67e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f67e-112">aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f67e-112">app</span></span>|[<span data-ttu-id="6f67e-113">appIdentity</span><span class="sxs-lookup"><span data-stu-id="6f67e-113">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="6f67e-114">Se o recurso que inicia a atividade for um aplicativo, essa propriedade indicará todas as informações relacionadas ao aplicativo, como appId, Name, servicePrincipalId, Name.</span><span class="sxs-lookup"><span data-stu-id="6f67e-114">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="6f67e-115">user</span><span class="sxs-lookup"><span data-stu-id="6f67e-115">user</span></span>|[<span data-ttu-id="6f67e-116">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6f67e-116">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="6f67e-117">Se o recurso que inicia a atividade for um usuário, essa propriedade indicará todas as informações relacionadas ao usuário, como userId, Name, UserPrinicpalName.</span><span class="sxs-lookup"><span data-stu-id="6f67e-117">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f67e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f67e-118">JSON representation</span></span>

<span data-ttu-id="6f67e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f67e-119">Here is a JSON representation of the resource.</span></span>

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

