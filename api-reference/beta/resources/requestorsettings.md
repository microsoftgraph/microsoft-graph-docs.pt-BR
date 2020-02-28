---
title: tipo complexo requestorSettings
description: Usada para a `requestorSettings` propriedade de uma política de atribuição de pacote do Access. Fornece configurações adicionais para selecionar quem pode criar uma solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad3205a6ef07c5cf09d8faeb07d19d760872d1e6
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331337"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="dc37d-104">tipo de recurso requestorSettings</span><span class="sxs-lookup"><span data-stu-id="dc37d-104">requestorSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc37d-105">Usado para a propriedade **requestorSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dc37d-105">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="dc37d-106">Fornece configurações adicionais para selecionar quem pode criar uma solicitação para um pacote do Access nessa política.</span><span class="sxs-lookup"><span data-stu-id="dc37d-106">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="dc37d-107">Quem pode solicitar</span><span class="sxs-lookup"><span data-stu-id="dc37d-107">Who can request</span></span> | <span data-ttu-id="dc37d-108">scopeType</span><span class="sxs-lookup"><span data-stu-id="dc37d-108">scopeType</span></span> | <span data-ttu-id="dc37d-109">coleção allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="dc37d-109">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="dc37d-110">Ninguém</span><span class="sxs-lookup"><span data-stu-id="dc37d-110">No one</span></span>|`NoSubjects`|<span data-ttu-id="dc37d-111">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="dc37d-111">empty array</span></span>|
|<span data-ttu-id="dc37d-112">Usuário individual específico em seu diretório</span><span class="sxs-lookup"><span data-stu-id="dc37d-112">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="dc37d-113">Únicousuário</span><span class="sxs-lookup"><span data-stu-id="dc37d-113">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="dc37d-114">Usuários em seu diretório que são membros de um grupo</span><span class="sxs-lookup"><span data-stu-id="dc37d-114">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="dc37d-115">groupMembers</span><span class="sxs-lookup"><span data-stu-id="dc37d-115">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="dc37d-116">Os usuários em seu diretório `userType` com o valor de`member`</span><span class="sxs-lookup"><span data-stu-id="dc37d-116">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="dc37d-117">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="dc37d-117">empty array</span></span>|
|<span data-ttu-id="dc37d-118">Usuários no seu diretório</span><span class="sxs-lookup"><span data-stu-id="dc37d-118">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="dc37d-119">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="dc37d-119">empty array</span></span>|
|<span data-ttu-id="dc37d-120">Usuários em outras organizações conectadas já configuradas</span><span class="sxs-lookup"><span data-stu-id="dc37d-120">Users in specific other connected organizations already configured</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="dc37d-121">connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="dc37d-121">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="dc37d-122">Usuários de outras organizações conectadas já configuradas</span><span class="sxs-lookup"><span data-stu-id="dc37d-122">Users from any other connected organizations already configured</span></span>|`AllExistingConnectedOrganizationSubjects`|<span data-ttu-id="dc37d-123">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="dc37d-123">empty array</span></span>|
|<span data-ttu-id="dc37d-124">Qualquer usuário</span><span class="sxs-lookup"><span data-stu-id="dc37d-124">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="dc37d-125">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="dc37d-125">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="dc37d-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc37d-126">Properties</span></span>

| <span data-ttu-id="dc37d-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc37d-127">Property</span></span>                     | <span data-ttu-id="dc37d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc37d-128">Type</span></span>                      | <span data-ttu-id="dc37d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc37d-129">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="dc37d-130">scopeType</span><span class="sxs-lookup"><span data-stu-id="dc37d-130">scopeType</span></span> |<span data-ttu-id="dc37d-131">String</span><span class="sxs-lookup"><span data-stu-id="dc37d-131">String</span></span> |<span data-ttu-id="dc37d-132">Quem pode solicitar.</span><span class="sxs-lookup"><span data-stu-id="dc37d-132">Who can request.</span></span> <span data-ttu-id="dc37d-133">Um dos `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` ou `AllExternalSubjects`.</span><span class="sxs-lookup"><span data-stu-id="dc37d-133">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="dc37d-134">acceptRequests</span><span class="sxs-lookup"><span data-stu-id="dc37d-134">acceptRequests</span></span> | <span data-ttu-id="dc37d-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="dc37d-135">Boolean</span></span> | <span data-ttu-id="dc37d-136">Indica se novas solicitações serão aceitas nessa política.</span><span class="sxs-lookup"><span data-stu-id="dc37d-136">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="dc37d-137">allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="dc37d-137">allowedRequestors</span></span> | <span data-ttu-id="dc37d-138">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="dc37d-138">[userSet](userset.md) collection</span></span>| <span data-ttu-id="dc37d-139">Os usuários que têm permissão para solicitar essa política, que podem ser [únicousuário](singleuser.md), [groupMembers](groupmembers.md)e [connectedOrganizationMembers](connectedorganizationmembers.md).</span><span class="sxs-lookup"><span data-stu-id="dc37d-139">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dc37d-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc37d-140">JSON representation</span></span>


<span data-ttu-id="dc37d-141">Veja a seguir uma representação JSON da propriedade **requestorSettings** de uma política, que permite aos membros de um grupo solicitar.</span><span class="sxs-lookup"><span data-stu-id="dc37d-141">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings",
  "baseType": ""
}-->

```json
{
  "scopeType": "SpecificDirectorySubjects",
  "acceptRequests": true,
  "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.groupMembers",
         "isBackup": false,
         "id": "string (identifier)",
         "description": "Authorized requestors"
       }
   ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
