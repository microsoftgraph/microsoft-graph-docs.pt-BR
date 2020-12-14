---
title: tipo de recurso aadUserConversationMemberResult
description: Recurso para a modelagem de respostas de operações em massa no aadUserConversationMember.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8251107c325bdbe2c5ff9e6df95a2d08277dde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663901"
---
# <a name="aaduserconversationmemberresult-resource-type"></a><span data-ttu-id="e2e83-103">tipo de recurso aadUserConversationMemberResult</span><span class="sxs-lookup"><span data-stu-id="e2e83-103">aadUserConversationMemberResult resource type</span></span>

<span data-ttu-id="e2e83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2e83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2e83-105">Representa a resposta individual para cada membro especificado em uma operação em massa que consiste em [aadUserConversationMember (s)](aadUserConversationMember.md) na solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2e83-105">Represents the individual response for each member specified in a bulk operation comprising of [aadUserConversationMember(s)](aadUserConversationMember.md) in the request.</span></span>
<span data-ttu-id="e2e83-106">Este recurso é a derivada do recurso [actionResultPart](actionresultpart.md) .</span><span class="sxs-lookup"><span data-stu-id="e2e83-106">This resource is the derivative of the [actionResultPart](actionresultpart.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="e2e83-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2e83-107">Properties</span></span>

| <span data-ttu-id="e2e83-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2e83-108">Property</span></span> | <span data-ttu-id="e2e83-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2e83-109">Type</span></span>   | <span data-ttu-id="e2e83-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2e83-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e2e83-111">userId</span><span class="sxs-lookup"><span data-stu-id="e2e83-111">userId</span></span>|`String`|<span data-ttu-id="e2e83-112">A ID de objeto do usuário do Azure AD que foi adicionada como parte da operação em massa.</span><span class="sxs-lookup"><span data-stu-id="e2e83-112">The user object ID of the Azure AD user that was being added as part of the bulk operation.</span></span>|
|<span data-ttu-id="e2e83-113">erro</span><span class="sxs-lookup"><span data-stu-id="e2e83-113">error</span></span>|[<span data-ttu-id="e2e83-114">publicError</span><span class="sxs-lookup"><span data-stu-id="e2e83-114">publicError</span></span>](publicerror.md) |<span data-ttu-id="e2e83-115">O erro que ocorreu, se houver, durante o andamento da operação em massa.</span><span class="sxs-lookup"><span data-stu-id="e2e83-115">The error that occurred, if any, during the course of the bulk operation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2e83-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2e83-116">JSON representation</span></span>

<span data-ttu-id="e2e83-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2e83-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserConversationMemberResult"
}-->

```json
{
    "userId": "string",
    "error": "microsoft.graph.publicError"
}
```

## <a name="see-also"></a><span data-ttu-id="e2e83-118">Confira também</span><span class="sxs-lookup"><span data-stu-id="e2e83-118">See also</span></span>

- [<span data-ttu-id="e2e83-119">Adicionar membros em massa à equipe</span><span class="sxs-lookup"><span data-stu-id="e2e83-119">Add members in bulk to team</span></span>](../api/conversationmembers-add.md)

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "actionResultPart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


