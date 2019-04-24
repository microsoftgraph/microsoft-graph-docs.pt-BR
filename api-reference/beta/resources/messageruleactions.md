---
title: Tipo de recurso messageRuleActions
description: Representa o conjunto de ações que estão disponíveis para uma regra.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a786a225bb9d439d60a29d2395b2d438975fc16c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523406"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="fc4fe-103">Tipo de recurso messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="fc4fe-103">messageRuleActions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc4fe-104">Representa o conjunto de ações que estão disponíveis para uma regra.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="fc4fe-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc4fe-105">Properties</span></span>
| <span data-ttu-id="fc4fe-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc4fe-106">Property</span></span>     | <span data-ttu-id="fc4fe-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc4fe-107">Type</span></span>   |<span data-ttu-id="fc4fe-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc4fe-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc4fe-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="fc4fe-109">assignCategories</span></span> | <span data-ttu-id="fc4fe-110">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc4fe-110">String collection</span></span> | <span data-ttu-id="fc4fe-111">Uma lista de categorias a serem atribuídas a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="fc4fe-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="fc4fe-112">copyToFolder</span></span> | <span data-ttu-id="fc4fe-113">String</span><span class="sxs-lookup"><span data-stu-id="fc4fe-113">String</span></span> | <span data-ttu-id="fc4fe-114">O ID de uma pasta para a qual uma mensagem deve ser copiada.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="fc4fe-115">delete</span><span class="sxs-lookup"><span data-stu-id="fc4fe-115">delete</span></span> | <span data-ttu-id="fc4fe-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="fc4fe-116">Boolean</span></span> | <span data-ttu-id="fc4fe-117">Indica se uma mensagem deve ser movida para a pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="fc4fe-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="fc4fe-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="fc4fe-119">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="fc4fe-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="fc4fe-120">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada como um anexo.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="fc4fe-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="fc4fe-121">forwardTo</span></span> | <span data-ttu-id="fc4fe-122">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="fc4fe-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="fc4fe-123">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="fc4fe-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="fc4fe-124">markAsRead</span></span> | <span data-ttu-id="fc4fe-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="fc4fe-125">Boolean</span></span> | <span data-ttu-id="fc4fe-126">Indica se uma mensagem deve ser marcada como lida.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="fc4fe-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="fc4fe-127">markImportance</span></span> | <span data-ttu-id="fc4fe-128">String</span><span class="sxs-lookup"><span data-stu-id="fc4fe-128">String</span></span> | <span data-ttu-id="fc4fe-129">Define a importância da mensagem, que pode ser: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="fc4fe-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="fc4fe-130">moveToFolder</span></span> |  <span data-ttu-id="fc4fe-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc4fe-131">String</span></span>| <span data-ttu-id="fc4fe-132">O ID da pasta para a qual uma mensagem será movida.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="fc4fe-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="fc4fe-133">permanentDelete</span></span> | <span data-ttu-id="fc4fe-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="fc4fe-134">Boolean</span></span> | <span data-ttu-id="fc4fe-135">Indica se uma mensagem deve ser excluída permanentemente e não salva na pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="fc4fe-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="fc4fe-136">redirectTo</span></span> | [<span data-ttu-id="fc4fe-137">recipient</span><span class="sxs-lookup"><span data-stu-id="fc4fe-137">recipient</span></span>](recipient.md) | <span data-ttu-id="fc4fe-138">Os endereço de email para o qual uma mensagem deve ser redirecionada.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-138">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="fc4fe-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="fc4fe-139">stopProcessingRules</span></span> | <span data-ttu-id="fc4fe-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc4fe-140">Boolean</span></span> | <span data-ttu-id="fc4fe-141">Indica se regras subsequentes devem ser avaliadas.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-141">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="fc4fe-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc4fe-142">JSON representation</span></span>
<span data-ttu-id="fc4fe-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc4fe-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messageruleactions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
