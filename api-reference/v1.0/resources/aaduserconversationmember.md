---
title: tipo de recurso aadUserConversationMember
description: Representa um usuário do Azure Active Directory em um chat ou canal.
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9714605cabbc25d3eeae7a68b2bc8f09d6131836
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873406"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="f9eec-103">tipo de recurso aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="f9eec-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="f9eec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9eec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9eec-105">Representa um usuário do Azure Active Directory em uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="f9eec-105">Represents an Azure Active Directory user in a [team](team.md).</span></span>
<span data-ttu-id="f9eec-106">Esse tipo é herdado do [conversationMember](conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="f9eec-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f9eec-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9eec-107">Properties</span></span>

| <span data-ttu-id="f9eec-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9eec-108">Property</span></span>   | <span data-ttu-id="f9eec-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9eec-109">Type</span></span> |<span data-ttu-id="f9eec-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9eec-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9eec-111">id</span><span class="sxs-lookup"><span data-stu-id="f9eec-111">id</span></span>|<span data-ttu-id="f9eec-112">String</span><span class="sxs-lookup"><span data-stu-id="f9eec-112">String</span></span>| <span data-ttu-id="f9eec-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9eec-113">Read-only.</span></span> <span data-ttu-id="f9eec-114">ID exclusivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9eec-114">Unique ID of the user.</span></span>|
|<span data-ttu-id="f9eec-115">displayName</span><span class="sxs-lookup"><span data-stu-id="f9eec-115">displayName</span></span>| <span data-ttu-id="f9eec-116">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9eec-116">string</span></span> | <span data-ttu-id="f9eec-117">O nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9eec-117">The display name of the user.</span></span> |
|<span data-ttu-id="f9eec-118">funções</span><span class="sxs-lookup"><span data-stu-id="f9eec-118">roles</span></span>| <span data-ttu-id="f9eec-119">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9eec-119">string collection</span></span> | <span data-ttu-id="f9eec-120">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="f9eec-120">The roles for that user.</span></span> |
|<span data-ttu-id="f9eec-121">userId</span><span class="sxs-lookup"><span data-stu-id="f9eec-121">userId</span></span>| <span data-ttu-id="f9eec-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9eec-122">string</span></span> | <span data-ttu-id="f9eec-123">O guid do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9eec-123">The guid of the user.</span></span> |
|<span data-ttu-id="f9eec-124">email</span><span class="sxs-lookup"><span data-stu-id="f9eec-124">email</span></span>| <span data-ttu-id="f9eec-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9eec-125">string</span></span>  | <span data-ttu-id="f9eec-126">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f9eec-126">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9eec-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9eec-127">JSON representation</span></span>

<span data-ttu-id="f9eec-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9eec-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
