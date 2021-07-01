---
title: Tipo de recurso teamworkTagIdentity
description: Representa uma marca em Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b9ea11746a98fba8bb209112c1cb6b1ed63fc954
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211064"
---
# <a name="teamworktagidentity-resource-type"></a><span data-ttu-id="9e124-103">Tipo de recurso teamworkTagIdentity</span><span class="sxs-lookup"><span data-stu-id="9e124-103">teamworkTagIdentity resource type</span></span>

<span data-ttu-id="9e124-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e124-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e124-105">Representa uma **marca** em Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="9e124-105">Represents a **tag** in Microsoft Teams.</span></span> <span data-ttu-id="9e124-106">As marcas permitem que os usuários se conectem rapidamente ao subconjunto de usuários em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="9e124-106">Tags allow users to quickly connect to subset of users in a team.</span></span> <span data-ttu-id="9e124-107">Para obter detalhes sobre o gerenciamento de marca Microsoft Teams, consulte [Manage tags in Microsoft Teams](/microsoftteams/manage-tags).</span><span class="sxs-lookup"><span data-stu-id="9e124-107">For details about tag management in Microsoft Teams, see [Manage tags in Microsoft Teams](/microsoftteams/manage-tags).</span></span>


<span data-ttu-id="9e124-108">Herda da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="9e124-108">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9e124-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e124-109">Properties</span></span>
|<span data-ttu-id="9e124-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e124-110">Property</span></span>|<span data-ttu-id="9e124-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e124-111">Type</span></span>|<span data-ttu-id="9e124-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e124-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e124-113">displayName</span><span class="sxs-lookup"><span data-stu-id="9e124-113">displayName</span></span>|<span data-ttu-id="9e124-114">String</span><span class="sxs-lookup"><span data-stu-id="9e124-114">String</span></span>|<span data-ttu-id="9e124-115">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="9e124-115">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="9e124-116">Nome de exibição da marca.</span><span class="sxs-lookup"><span data-stu-id="9e124-116">Display name of the tag.</span></span>|
|<span data-ttu-id="9e124-117">id</span><span class="sxs-lookup"><span data-stu-id="9e124-117">id</span></span>|<span data-ttu-id="9e124-118">String</span><span class="sxs-lookup"><span data-stu-id="9e124-118">String</span></span>|<span data-ttu-id="9e124-119">Herdado da [identidade](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="9e124-119">Inherited from [identity](../resources/identity.md).</span></span> <span data-ttu-id="9e124-120">ID da marca.</span><span class="sxs-lookup"><span data-stu-id="9e124-120">ID of the tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e124-121">Relações</span><span class="sxs-lookup"><span data-stu-id="9e124-121">Relationships</span></span>
<span data-ttu-id="9e124-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e124-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e124-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e124-123">JSON representation</span></span>
<span data-ttu-id="9e124-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e124-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkTagIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagIdentity",
  "id": "String (identifier)",
  "displayName": "String"
}
```

