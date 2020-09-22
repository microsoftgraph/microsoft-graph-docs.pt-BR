---
title: Tipo de recurso messageRuleActions
description: Representa o conjunto de ações que estão disponíveis para uma regra.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: aae9420f3d1b6e329a007eda3917ce7eaa8c4dda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971534"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="a02d7-103">Tipo de recurso messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="a02d7-103">messageRuleActions resource type</span></span>

<span data-ttu-id="a02d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a02d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a02d7-105">Representa o conjunto de ações que estão disponíveis para uma regra.</span><span class="sxs-lookup"><span data-stu-id="a02d7-105">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="a02d7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a02d7-106">Properties</span></span>
| <span data-ttu-id="a02d7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a02d7-107">Property</span></span>     | <span data-ttu-id="a02d7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a02d7-108">Type</span></span>   |<span data-ttu-id="a02d7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a02d7-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a02d7-110">assignCategories</span><span class="sxs-lookup"><span data-stu-id="a02d7-110">assignCategories</span></span> | <span data-ttu-id="a02d7-111">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a02d7-111">String collection</span></span> | <span data-ttu-id="a02d7-112">Uma lista de categorias a serem atribuídas a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="a02d7-112">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="a02d7-113">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="a02d7-113">copyToFolder</span></span> | <span data-ttu-id="a02d7-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a02d7-114">String</span></span> | <span data-ttu-id="a02d7-115">O ID de uma pasta para a qual uma mensagem deve ser copiada.</span><span class="sxs-lookup"><span data-stu-id="a02d7-115">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="a02d7-116">delete</span><span class="sxs-lookup"><span data-stu-id="a02d7-116">delete</span></span> | <span data-ttu-id="a02d7-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a02d7-117">Boolean</span></span> | <span data-ttu-id="a02d7-118">Indica se uma mensagem deve ser movida para a pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="a02d7-118">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="a02d7-119">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="a02d7-119">forwardAsAttachmentTo</span></span> | <span data-ttu-id="a02d7-120">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a02d7-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="a02d7-121">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada como um anexo.</span><span class="sxs-lookup"><span data-stu-id="a02d7-121">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="a02d7-122">forwardTo</span><span class="sxs-lookup"><span data-stu-id="a02d7-122">forwardTo</span></span> | <span data-ttu-id="a02d7-123">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a02d7-123">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="a02d7-124">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada.</span><span class="sxs-lookup"><span data-stu-id="a02d7-124">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="a02d7-125">markAsRead</span><span class="sxs-lookup"><span data-stu-id="a02d7-125">markAsRead</span></span> | <span data-ttu-id="a02d7-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="a02d7-126">Boolean</span></span> | <span data-ttu-id="a02d7-127">Indica se uma mensagem deve ser marcada como lida.</span><span class="sxs-lookup"><span data-stu-id="a02d7-127">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="a02d7-128">markImportance</span><span class="sxs-lookup"><span data-stu-id="a02d7-128">markImportance</span></span> | <span data-ttu-id="a02d7-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a02d7-129">String</span></span> | <span data-ttu-id="a02d7-130">Define a importância da mensagem, que pode ser: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="a02d7-130">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="a02d7-131">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="a02d7-131">moveToFolder</span></span> |  <span data-ttu-id="a02d7-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a02d7-132">String</span></span>| <span data-ttu-id="a02d7-133">O ID da pasta para a qual uma mensagem será movida.</span><span class="sxs-lookup"><span data-stu-id="a02d7-133">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="a02d7-134">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="a02d7-134">permanentDelete</span></span> | <span data-ttu-id="a02d7-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a02d7-135">Boolean</span></span> | <span data-ttu-id="a02d7-136">Indica se uma mensagem deve ser excluída permanentemente e não salva na pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="a02d7-136">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="a02d7-137">redirectTo</span><span class="sxs-lookup"><span data-stu-id="a02d7-137">redirectTo</span></span> | [<span data-ttu-id="a02d7-138">recipient</span><span class="sxs-lookup"><span data-stu-id="a02d7-138">recipient</span></span>](recipient.md) | <span data-ttu-id="a02d7-139">Os endereço de email para o qual uma mensagem deve ser redirecionada.</span><span class="sxs-lookup"><span data-stu-id="a02d7-139">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="a02d7-140">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="a02d7-140">stopProcessingRules</span></span> | <span data-ttu-id="a02d7-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="a02d7-141">Boolean</span></span> | <span data-ttu-id="a02d7-142">Indica se regras subsequentes devem ser avaliadas.</span><span class="sxs-lookup"><span data-stu-id="a02d7-142">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a02d7-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a02d7-143">JSON representation</span></span>
<span data-ttu-id="a02d7-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a02d7-144">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


