---
title: Tipo de recurso teamworkApplicationIdentity
description: Representa um aplicativo em Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 67e1ed4365febae44032c09d94656d2e3ac0b504
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211066"
---
# <a name="teamworkapplicationidentity-resource-type"></a><span data-ttu-id="918f7-103">Tipo de recurso teamworkApplicationIdentity</span><span class="sxs-lookup"><span data-stu-id="918f7-103">teamworkApplicationIdentity resource type</span></span>

<span data-ttu-id="918f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="918f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="918f7-105">Representa um **aplicativo** em Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="918f7-105">Represents an **application** in Microsoft Teams.</span></span> <span data-ttu-id="918f7-106">`teamworkApplicationIdentity` é usado para representar bots e webhooks de saída @mentioned mensagens.</span><span class="sxs-lookup"><span data-stu-id="918f7-106">`teamworkApplicationIdentity` is used to represent bots and outgoing webhooks @mentioned in messages.</span></span>


<span data-ttu-id="918f7-107">Herda da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="918f7-107">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="918f7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="918f7-108">Properties</span></span>
|<span data-ttu-id="918f7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="918f7-109">Property</span></span>|<span data-ttu-id="918f7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="918f7-110">Type</span></span>|<span data-ttu-id="918f7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="918f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="918f7-112">applicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="918f7-112">applicationIdentityType</span></span>|<span data-ttu-id="918f7-113">teamworkApplicationIdentityType</span><span class="sxs-lookup"><span data-stu-id="918f7-113">teamworkApplicationIdentityType</span></span>| <span data-ttu-id="918f7-114">Tipo de aplicativo referenciado.</span><span class="sxs-lookup"><span data-stu-id="918f7-114">Type of application that is referenced.</span></span> <span data-ttu-id="918f7-115">Os valores possíveis são: `aadApplication` , , , , e `bot` `tenantBot` `office365Connector` `outgoingWebhook` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="918f7-115">Possible values are: `aadApplication`, `bot`, `tenantBot`, `office365Connector`, `outgoingWebhook`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="918f7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="918f7-116">displayName</span></span>|<span data-ttu-id="918f7-117">String</span><span class="sxs-lookup"><span data-stu-id="918f7-117">String</span></span>|<span data-ttu-id="918f7-118">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="918f7-118">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="918f7-119">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="918f7-119">Display name of the application.</span></span> <span data-ttu-id="918f7-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="918f7-120">Optional.</span></span>|
|<span data-ttu-id="918f7-121">id</span><span class="sxs-lookup"><span data-stu-id="918f7-121">id</span></span>|<span data-ttu-id="918f7-122">String</span><span class="sxs-lookup"><span data-stu-id="918f7-122">String</span></span>|<span data-ttu-id="918f7-123">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="918f7-123">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="918f7-124">ID do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="918f7-124">ID of the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="918f7-125">Relações</span><span class="sxs-lookup"><span data-stu-id="918f7-125">Relationships</span></span>
<span data-ttu-id="918f7-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="918f7-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="918f7-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="918f7-127">JSON representation</span></span>
<span data-ttu-id="918f7-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="918f7-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkApplicationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkApplicationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "applicationIdentityType": "String"
}
```

