---
title: Tipo de recurso messageRuleActions
description: Representa o conjunto de ações que estão disponíveis para uma regra.
author: angelgolfer-ms
ms.openlocfilehash: c65e950fbe440ba6e453856b034036fada657f0b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347345"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="9a9ed-103">Tipo de recurso messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="9a9ed-103">messageRuleActions resource type</span></span>


<span data-ttu-id="9a9ed-104">Representa o conjunto de ações que estão disponíveis para uma regra.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="9a9ed-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a9ed-105">Properties</span></span>
| <span data-ttu-id="9a9ed-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a9ed-106">Property</span></span>     | <span data-ttu-id="9a9ed-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a9ed-107">Type</span></span>   |<span data-ttu-id="9a9ed-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a9ed-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a9ed-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="9a9ed-109">assignCategories</span></span> | <span data-ttu-id="9a9ed-110">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a9ed-110">String collection</span></span> | <span data-ttu-id="9a9ed-111">Uma lista de categorias a serem atribuídas a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="9a9ed-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="9a9ed-112">copyToFolder</span></span> | <span data-ttu-id="9a9ed-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a9ed-113">String</span></span> | <span data-ttu-id="9a9ed-114">O ID de uma pasta para a qual uma mensagem deve ser copiada.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="9a9ed-115">delete</span><span class="sxs-lookup"><span data-stu-id="9a9ed-115">delete</span></span> | <span data-ttu-id="9a9ed-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a9ed-116">Boolean</span></span> | <span data-ttu-id="9a9ed-117">Indica se uma mensagem deve ser movida para a pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="9a9ed-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="9a9ed-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="9a9ed-119">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="9a9ed-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="9a9ed-120">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada como um anexo.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="9a9ed-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="9a9ed-121">forwardTo</span></span> | <span data-ttu-id="9a9ed-122">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="9a9ed-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="9a9ed-123">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="9a9ed-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="9a9ed-124">markAsRead</span></span> | <span data-ttu-id="9a9ed-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a9ed-125">Boolean</span></span> | <span data-ttu-id="9a9ed-126">Indica se uma mensagem deve ser marcada como lida.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="9a9ed-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="9a9ed-127">markImportance</span></span> | <span data-ttu-id="9a9ed-128">importance</span><span class="sxs-lookup"><span data-stu-id="9a9ed-128">importance</span></span> | <span data-ttu-id="9a9ed-129">Define a importância da mensagem, que pode ser: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="9a9ed-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="9a9ed-130">moveToFolder</span></span> |  <span data-ttu-id="9a9ed-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a9ed-131">String</span></span>| <span data-ttu-id="9a9ed-132">O ID da pasta para a qual uma mensagem será movida.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="9a9ed-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="9a9ed-133">permanentDelete</span></span> | <span data-ttu-id="9a9ed-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a9ed-134">Boolean</span></span> | <span data-ttu-id="9a9ed-135">Indica se uma mensagem deve ser excluída permanentemente e não salva na pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="9a9ed-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="9a9ed-136">redirectTo</span></span> | <span data-ttu-id="9a9ed-137">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="9a9ed-137">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="9a9ed-138">Os endereços de email ao qual uma mensagem deve ser redirecionada.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-138">The email addresses to which a message should be redirected.</span></span> |
| <span data-ttu-id="9a9ed-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="9a9ed-139">stopProcessingRules</span></span> | <span data-ttu-id="9a9ed-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a9ed-140">Boolean</span></span> | <span data-ttu-id="9a9ed-141">Indica se regras subsequentes devem ser avaliadas.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-141">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a9ed-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a9ed-142">JSON representation</span></span>
<span data-ttu-id="9a9ed-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a9ed-143">Here is a JSON representation of the resource.</span></span>

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
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->