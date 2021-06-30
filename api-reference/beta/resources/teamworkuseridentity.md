---
title: tipo de recurso teamworkUserIdentity
description: Representa um usuário no Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b0c50856a2b7051a631cd14ab3985cd8724bfe4c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211243"
---
# <a name="teamworkuseridentity-resource-type"></a><span data-ttu-id="4455b-103">tipo de recurso teamworkUserIdentity</span><span class="sxs-lookup"><span data-stu-id="4455b-103">teamworkUserIdentity resource type</span></span>

<span data-ttu-id="4455b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4455b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4455b-105">Representa um **usuário** em Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4455b-105">Represents a **user** in Microsoft Teams.</span></span>


<span data-ttu-id="4455b-106">Herda da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="4455b-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4455b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4455b-107">Properties</span></span>
|<span data-ttu-id="4455b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4455b-108">Property</span></span>|<span data-ttu-id="4455b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4455b-109">Type</span></span>|<span data-ttu-id="4455b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4455b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4455b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4455b-111">displayName</span></span>|<span data-ttu-id="4455b-112">String</span><span class="sxs-lookup"><span data-stu-id="4455b-112">String</span></span>|<span data-ttu-id="4455b-113">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="4455b-113">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="4455b-114">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="4455b-114">Display name of the user.</span></span> <span data-ttu-id="4455b-115">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4455b-115">Optional.</span></span>|
|<span data-ttu-id="4455b-116">id</span><span class="sxs-lookup"><span data-stu-id="4455b-116">id</span></span>|<span data-ttu-id="4455b-117">String</span><span class="sxs-lookup"><span data-stu-id="4455b-117">String</span></span>|<span data-ttu-id="4455b-118">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="4455b-118">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="4455b-119">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="4455b-119">ID of the user.</span></span> |
|<span data-ttu-id="4455b-120">userIdentityType</span><span class="sxs-lookup"><span data-stu-id="4455b-120">userIdentityType</span></span>|<span data-ttu-id="4455b-121">teamworkUserIdentityType</span><span class="sxs-lookup"><span data-stu-id="4455b-121">teamworkUserIdentityType</span></span>| <span data-ttu-id="4455b-122">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="4455b-122">Type of user.</span></span> <span data-ttu-id="4455b-123">Os valores possíveis são: `aadUser` , , , , , e `onPremiseAadUser` `anonymousGuest` `federatedUser` `personalMicrosoftAccountUser` `skypeUser` `phoneUser` .</span><span class="sxs-lookup"><span data-stu-id="4455b-123">Possible values are: `aadUser`, `onPremiseAadUser`, `anonymousGuest`, `federatedUser`, `personalMicrosoftAccountUser`, `skypeUser`, and `phoneUser`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4455b-124">Relações</span><span class="sxs-lookup"><span data-stu-id="4455b-124">Relationships</span></span>
<span data-ttu-id="4455b-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4455b-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4455b-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4455b-126">JSON representation</span></span>
<span data-ttu-id="4455b-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4455b-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkUserIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkUserIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "userIdentityType": "String"
}
```

