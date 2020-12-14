---
title: tipo de recurso actionResultType
description: Tipo abstrato para a modelagem de respostas de operações em massa.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a092fa4a322d0d207550947559cb5dfff4ad4625
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663996"
---
# <a name="actionresultpart-resource-type"></a><span data-ttu-id="be658-103">tipo de recurso actionResultPart</span><span class="sxs-lookup"><span data-stu-id="be658-103">actionResultPart resource type</span></span>

<span data-ttu-id="be658-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be658-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be658-105">Um tipo abstrato que serve como base para a modelagem de respostas de operações em massa.</span><span class="sxs-lookup"><span data-stu-id="be658-105">An abstract type that serves as a base for modeling responses of bulk operations.</span></span> <span data-ttu-id="be658-106">A propriedade **Error** é preenchida seletivamente com base em se a resposta representa um erro.</span><span class="sxs-lookup"><span data-stu-id="be658-106">The **error** property is selectively populated based on whether the response represents an error.</span></span>

## <a name="properties"></a><span data-ttu-id="be658-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be658-107">Properties</span></span>

| <span data-ttu-id="be658-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be658-108">Property</span></span> | <span data-ttu-id="be658-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="be658-109">Type</span></span>   | <span data-ttu-id="be658-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="be658-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="be658-111">erro</span><span class="sxs-lookup"><span data-stu-id="be658-111">error</span></span>|[<span data-ttu-id="be658-112">publicError</span><span class="sxs-lookup"><span data-stu-id="be658-112">publicError</span></span>](publicerror.md) |<span data-ttu-id="be658-113">O erro que ocorreu, se houver, durante o andamento da operação em massa.</span><span class="sxs-lookup"><span data-stu-id="be658-113">The error that occurred, if any, during the course of the bulk operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be658-114">Relações</span><span class="sxs-lookup"><span data-stu-id="be658-114">Relationships</span></span>
<span data-ttu-id="be658-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be658-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be658-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be658-116">JSON representation</span></span>
<span data-ttu-id="be658-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be658-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.actionResultPart"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.actionResultPart",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  }
}
```
## <a name="see-also"></a><span data-ttu-id="be658-118">Confira também</span><span class="sxs-lookup"><span data-stu-id="be658-118">See also</span></span>

- [<span data-ttu-id="be658-119">aadUserConversationMemberResult</span><span class="sxs-lookup"><span data-stu-id="be658-119">aadUserConversationMemberResult</span></span>](aadUserConversationMemberResult.md)
- [<span data-ttu-id="be658-120">Adicionar membros em massa à equipe</span><span class="sxs-lookup"><span data-stu-id="be658-120">Add members in bulk to team</span></span>](../api/conversationmembers-add.md)

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


