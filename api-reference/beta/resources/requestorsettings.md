---
title: Tipo complexo requestorSettings
description: Usado para a propriedade `requestorSettings` de uma política de atribuição de pacote de acesso. Fornece configurações adicionais para selecionar quem pode criar uma solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a9bd91605d106b488de21f29baefe4b31d28f323
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133725"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="fa743-104">Tipo de recurso requestorSettings</span><span class="sxs-lookup"><span data-stu-id="fa743-104">requestorSettings resource type</span></span>

<span data-ttu-id="fa743-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa743-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa743-106">Usado para a **propriedade requestorSettings** de uma política [de atribuição de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fa743-106">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="fa743-107">Fornece configurações adicionais para selecionar quem pode criar uma solicitação para um pacote de acesso nessa política.</span><span class="sxs-lookup"><span data-stu-id="fa743-107">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="fa743-108">Quem pode solicitar</span><span class="sxs-lookup"><span data-stu-id="fa743-108">Who can request</span></span> | <span data-ttu-id="fa743-109">scopeType</span><span class="sxs-lookup"><span data-stu-id="fa743-109">scopeType</span></span> | <span data-ttu-id="fa743-110">Coleção allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="fa743-110">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="fa743-111">Ninguém</span><span class="sxs-lookup"><span data-stu-id="fa743-111">No one</span></span>|`NoSubjects`|<span data-ttu-id="fa743-112">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="fa743-112">empty array</span></span>|
|<span data-ttu-id="fa743-113">Usuário individual específico em seu diretório</span><span class="sxs-lookup"><span data-stu-id="fa743-113">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="fa743-114">singleUser</span><span class="sxs-lookup"><span data-stu-id="fa743-114">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="fa743-115">Usuários em seu diretório que são membros de um grupo</span><span class="sxs-lookup"><span data-stu-id="fa743-115">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="fa743-116">groupMembers</span><span class="sxs-lookup"><span data-stu-id="fa743-116">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="fa743-117">Usuários em seu diretório com `userType` valor de `member`</span><span class="sxs-lookup"><span data-stu-id="fa743-117">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="fa743-118">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="fa743-118">empty array</span></span>|
|<span data-ttu-id="fa743-119">Usuários em seu diretório</span><span class="sxs-lookup"><span data-stu-id="fa743-119">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="fa743-120">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="fa743-120">empty array</span></span>|
|<span data-ttu-id="fa743-121">Usuários em organizações conectadas específicas</span><span class="sxs-lookup"><span data-stu-id="fa743-121">Users in specific connected organizations</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="fa743-122">connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="fa743-122">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="fa743-123">Usuários de qualquer organização conectada que tenham a propriedade de estado da organização conectada definida como `configured` .</span><span class="sxs-lookup"><span data-stu-id="fa743-123">Users from any connected organizations that have the state property of the connected organization set to `configured`.</span></span>|`AllConfiguredConnectedOrganizationSubjects`|<span data-ttu-id="fa743-124">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="fa743-124">empty array</span></span>|
|<span data-ttu-id="fa743-125">Qualquer usuário</span><span class="sxs-lookup"><span data-stu-id="fa743-125">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="fa743-126">matriz vazia</span><span class="sxs-lookup"><span data-stu-id="fa743-126">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="fa743-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa743-127">Properties</span></span>

| <span data-ttu-id="fa743-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa743-128">Property</span></span>                     | <span data-ttu-id="fa743-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa743-129">Type</span></span>                      | <span data-ttu-id="fa743-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa743-130">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="fa743-131">scopeType</span><span class="sxs-lookup"><span data-stu-id="fa743-131">scopeType</span></span> |<span data-ttu-id="fa743-132">String</span><span class="sxs-lookup"><span data-stu-id="fa743-132">String</span></span> |<span data-ttu-id="fa743-133">Quem pode solicitar.</span><span class="sxs-lookup"><span data-stu-id="fa743-133">Who can request.</span></span> <span data-ttu-id="fa743-134">Um de `NoSubjects` , , , , ou `SpecificDirectorySubjects` `SpecificConnectedOrganizationSubjects` `AllConfiguredConnectedOrganizationSubjects` `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` `AllExternalSubjects` .</span><span class="sxs-lookup"><span data-stu-id="fa743-134">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllConfiguredConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="fa743-135">acceptRequests</span><span class="sxs-lookup"><span data-stu-id="fa743-135">acceptRequests</span></span> | <span data-ttu-id="fa743-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa743-136">Boolean</span></span> | <span data-ttu-id="fa743-137">Indica se novas solicitações são aceitas nesta política.</span><span class="sxs-lookup"><span data-stu-id="fa743-137">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="fa743-138">allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="fa743-138">allowedRequestors</span></span> | <span data-ttu-id="fa743-139">[Coleção userSet](userset.md)</span><span class="sxs-lookup"><span data-stu-id="fa743-139">[userSet](userset.md) collection</span></span>| <span data-ttu-id="fa743-140">Os usuários que têm permissão para solicitar nesta política, que pode ser [singleUser](singleuser.md), [groupMembers](groupmembers.md)e [connectedOrganizationMembers](connectedorganizationmembers.md).</span><span class="sxs-lookup"><span data-stu-id="fa743-140">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa743-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa743-141">JSON representation</span></span>


<span data-ttu-id="fa743-142">A seguir está uma representação JSON da **propriedade requestorSettings** de uma política, que permite que os membros de um grupo solicitem.</span><span class="sxs-lookup"><span data-stu-id="fa743-142">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings"
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


