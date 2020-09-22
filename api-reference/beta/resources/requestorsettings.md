---
title: tipo complexo requestorSettings
description: Usada para a `requestorSettings` propriedade de uma política de atribuição de pacote do Access. Fornece configurações adicionais para selecionar quem pode criar uma solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aee297f36538ca45183e0c3185f35c8f340d8631
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026310"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="3813c-104">tipo de recurso requestorSettings</span><span class="sxs-lookup"><span data-stu-id="3813c-104">requestorSettings resource type</span></span>

<span data-ttu-id="3813c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3813c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3813c-106">Usado para a propriedade **requestorSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="3813c-106">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="3813c-107">Fornece configurações adicionais para selecionar quem pode criar uma solicitação para um pacote do Access nessa política.</span><span class="sxs-lookup"><span data-stu-id="3813c-107">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="3813c-108">Quem pode solicitar</span><span class="sxs-lookup"><span data-stu-id="3813c-108">Who can request</span></span> | <span data-ttu-id="3813c-109">scopeType</span><span class="sxs-lookup"><span data-stu-id="3813c-109">scopeType</span></span> | <span data-ttu-id="3813c-110">coleção allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="3813c-110">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="3813c-111">Ninguém</span><span class="sxs-lookup"><span data-stu-id="3813c-111">No one</span></span>|`NoSubjects`|<span data-ttu-id="3813c-112">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="3813c-112">empty array</span></span>|
|<span data-ttu-id="3813c-113">Usuário individual específico em seu diretório</span><span class="sxs-lookup"><span data-stu-id="3813c-113">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="3813c-114">Únicousuário</span><span class="sxs-lookup"><span data-stu-id="3813c-114">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="3813c-115">Usuários em seu diretório que são membros de um grupo</span><span class="sxs-lookup"><span data-stu-id="3813c-115">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="3813c-116">groupMembers</span><span class="sxs-lookup"><span data-stu-id="3813c-116">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="3813c-117">Os usuários em seu diretório com o `userType` valor de `member`</span><span class="sxs-lookup"><span data-stu-id="3813c-117">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="3813c-118">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="3813c-118">empty array</span></span>|
|<span data-ttu-id="3813c-119">Usuários no seu diretório</span><span class="sxs-lookup"><span data-stu-id="3813c-119">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="3813c-120">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="3813c-120">empty array</span></span>|
|<span data-ttu-id="3813c-121">Usuários em organizações conectadas específicas</span><span class="sxs-lookup"><span data-stu-id="3813c-121">Users in specific connected organizations</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="3813c-122">connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="3813c-122">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="3813c-123">Usuários de todas as organizações conectadas que têm a propriedade State da organização conectada definida como `configured` .</span><span class="sxs-lookup"><span data-stu-id="3813c-123">Users from any connected organizations that have the state property of the connected organization set to `configured`.</span></span>|`AllConfiguredConnectedOrganizationSubjects`|<span data-ttu-id="3813c-124">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="3813c-124">empty array</span></span>|
|<span data-ttu-id="3813c-125">Qualquer usuário</span><span class="sxs-lookup"><span data-stu-id="3813c-125">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="3813c-126">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="3813c-126">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="3813c-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3813c-127">Properties</span></span>

| <span data-ttu-id="3813c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3813c-128">Property</span></span>                     | <span data-ttu-id="3813c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3813c-129">Type</span></span>                      | <span data-ttu-id="3813c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3813c-130">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="3813c-131">scopeType</span><span class="sxs-lookup"><span data-stu-id="3813c-131">scopeType</span></span> |<span data-ttu-id="3813c-132">String</span><span class="sxs-lookup"><span data-stu-id="3813c-132">String</span></span> |<span data-ttu-id="3813c-133">Quem pode solicitar.</span><span class="sxs-lookup"><span data-stu-id="3813c-133">Who can request.</span></span> <span data-ttu-id="3813c-134">Um dos `NoSubjects` , `SpecificDirectorySubjects` , `SpecificConnectedOrganizationSubjects` , `AllExistingConnectedOrganizationSubjects` , `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` ou `AllExternalSubjects` .</span><span class="sxs-lookup"><span data-stu-id="3813c-134">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="3813c-135">acceptRequests</span><span class="sxs-lookup"><span data-stu-id="3813c-135">acceptRequests</span></span> | <span data-ttu-id="3813c-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="3813c-136">Boolean</span></span> | <span data-ttu-id="3813c-137">Indica se novas solicitações serão aceitas nessa política.</span><span class="sxs-lookup"><span data-stu-id="3813c-137">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="3813c-138">allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="3813c-138">allowedRequestors</span></span> | <span data-ttu-id="3813c-139">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="3813c-139">[userSet](userset.md) collection</span></span>| <span data-ttu-id="3813c-140">Os usuários que têm permissão para solicitar essa política, que podem ser [únicousuário](singleuser.md), [groupMembers](groupmembers.md)e [connectedOrganizationMembers](connectedorganizationmembers.md).</span><span class="sxs-lookup"><span data-stu-id="3813c-140">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3813c-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3813c-141">JSON representation</span></span>


<span data-ttu-id="3813c-142">Veja a seguir uma representação JSON da propriedade **requestorSettings** de uma política, que permite aos membros de um grupo solicitar.</span><span class="sxs-lookup"><span data-stu-id="3813c-142">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

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


