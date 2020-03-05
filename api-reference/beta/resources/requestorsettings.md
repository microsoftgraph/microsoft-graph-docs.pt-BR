---
title: tipo complexo requestorSettings
description: Usada para a `requestorSettings` propriedade de uma política de atribuição de pacote do Access. Fornece configurações adicionais para selecionar quem pode criar uma solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b52f3276185f819ccd0e7149dbd5420b4f6e1781
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521114"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="132cf-104">tipo de recurso requestorSettings</span><span class="sxs-lookup"><span data-stu-id="132cf-104">requestorSettings resource type</span></span>

<span data-ttu-id="132cf-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="132cf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="132cf-106">Usado para a propriedade **requestorSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="132cf-106">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="132cf-107">Fornece configurações adicionais para selecionar quem pode criar uma solicitação para um pacote do Access nessa política.</span><span class="sxs-lookup"><span data-stu-id="132cf-107">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="132cf-108">Quem pode solicitar</span><span class="sxs-lookup"><span data-stu-id="132cf-108">Who can request</span></span> | <span data-ttu-id="132cf-109">scopeType</span><span class="sxs-lookup"><span data-stu-id="132cf-109">scopeType</span></span> | <span data-ttu-id="132cf-110">coleção allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="132cf-110">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="132cf-111">Ninguém</span><span class="sxs-lookup"><span data-stu-id="132cf-111">No one</span></span>|`NoSubjects`|<span data-ttu-id="132cf-112">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="132cf-112">empty array</span></span>|
|<span data-ttu-id="132cf-113">Usuário individual específico em seu diretório</span><span class="sxs-lookup"><span data-stu-id="132cf-113">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="132cf-114">Únicousuário</span><span class="sxs-lookup"><span data-stu-id="132cf-114">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="132cf-115">Usuários em seu diretório que são membros de um grupo</span><span class="sxs-lookup"><span data-stu-id="132cf-115">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="132cf-116">groupMembers</span><span class="sxs-lookup"><span data-stu-id="132cf-116">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="132cf-117">Os usuários em seu diretório `userType` com o valor de`member`</span><span class="sxs-lookup"><span data-stu-id="132cf-117">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="132cf-118">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="132cf-118">empty array</span></span>|
|<span data-ttu-id="132cf-119">Usuários no seu diretório</span><span class="sxs-lookup"><span data-stu-id="132cf-119">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="132cf-120">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="132cf-120">empty array</span></span>|
|<span data-ttu-id="132cf-121">Usuários em outras organizações conectadas já configuradas</span><span class="sxs-lookup"><span data-stu-id="132cf-121">Users in specific other connected organizations already configured</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="132cf-122">connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="132cf-122">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="132cf-123">Usuários de outras organizações conectadas já configuradas</span><span class="sxs-lookup"><span data-stu-id="132cf-123">Users from any other connected organizations already configured</span></span>|`AllExistingConnectedOrganizationSubjects`|<span data-ttu-id="132cf-124">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="132cf-124">empty array</span></span>|
|<span data-ttu-id="132cf-125">Qualquer usuário</span><span class="sxs-lookup"><span data-stu-id="132cf-125">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="132cf-126">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="132cf-126">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="132cf-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="132cf-127">Properties</span></span>

| <span data-ttu-id="132cf-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="132cf-128">Property</span></span>                     | <span data-ttu-id="132cf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="132cf-129">Type</span></span>                      | <span data-ttu-id="132cf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="132cf-130">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="132cf-131">scopeType</span><span class="sxs-lookup"><span data-stu-id="132cf-131">scopeType</span></span> |<span data-ttu-id="132cf-132">String</span><span class="sxs-lookup"><span data-stu-id="132cf-132">String</span></span> |<span data-ttu-id="132cf-133">Quem pode solicitar.</span><span class="sxs-lookup"><span data-stu-id="132cf-133">Who can request.</span></span> <span data-ttu-id="132cf-134">Um dos `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` ou `AllExternalSubjects`.</span><span class="sxs-lookup"><span data-stu-id="132cf-134">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="132cf-135">acceptRequests</span><span class="sxs-lookup"><span data-stu-id="132cf-135">acceptRequests</span></span> | <span data-ttu-id="132cf-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="132cf-136">Boolean</span></span> | <span data-ttu-id="132cf-137">Indica se novas solicitações serão aceitas nessa política.</span><span class="sxs-lookup"><span data-stu-id="132cf-137">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="132cf-138">allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="132cf-138">allowedRequestors</span></span> | <span data-ttu-id="132cf-139">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="132cf-139">[userSet](userset.md) collection</span></span>| <span data-ttu-id="132cf-140">Os usuários que têm permissão para solicitar essa política, que podem ser [únicousuário](singleuser.md), [groupMembers](groupmembers.md)e [connectedOrganizationMembers](connectedorganizationmembers.md).</span><span class="sxs-lookup"><span data-stu-id="132cf-140">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="132cf-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="132cf-141">JSON representation</span></span>


<span data-ttu-id="132cf-142">Veja a seguir uma representação JSON da propriedade **requestorSettings** de uma política, que permite aos membros de um grupo solicitar.</span><span class="sxs-lookup"><span data-stu-id="132cf-142">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

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
