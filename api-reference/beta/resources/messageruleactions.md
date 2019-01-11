---
title: Tipo de recurso messageRuleActions
description: Representa o conjunto de ações que estão disponíveis para uma regra.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f6a78442dc82cade6b7e6d9a793fb6e49b3a1beb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889037"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="51e37-103">Tipo de recurso messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="51e37-103">messageRuleActions resource type</span></span>

> <span data-ttu-id="51e37-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51e37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51e37-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51e37-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51e37-106">Representa o conjunto de ações que estão disponíveis para uma regra.</span><span class="sxs-lookup"><span data-stu-id="51e37-106">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="51e37-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51e37-107">Properties</span></span>
| <span data-ttu-id="51e37-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51e37-108">Property</span></span>     | <span data-ttu-id="51e37-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="51e37-109">Type</span></span>   |<span data-ttu-id="51e37-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e37-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51e37-111">assignCategories</span><span class="sxs-lookup"><span data-stu-id="51e37-111">assignCategories</span></span> | <span data-ttu-id="51e37-112">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e37-112">String collection</span></span> | <span data-ttu-id="51e37-113">Uma lista de categorias a serem atribuídas a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="51e37-113">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="51e37-114">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="51e37-114">copyToFolder</span></span> | <span data-ttu-id="51e37-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e37-115">String</span></span> | <span data-ttu-id="51e37-116">O ID de uma pasta para a qual uma mensagem deve ser copiada.</span><span class="sxs-lookup"><span data-stu-id="51e37-116">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="51e37-117">delete</span><span class="sxs-lookup"><span data-stu-id="51e37-117">delete</span></span> | <span data-ttu-id="51e37-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="51e37-118">Boolean</span></span> | <span data-ttu-id="51e37-119">Indica se uma mensagem deve ser movida para a pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="51e37-119">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="51e37-120">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="51e37-120">forwardAsAttachmentTo</span></span> | <span data-ttu-id="51e37-121">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="51e37-121">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="51e37-122">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada como um anexo.</span><span class="sxs-lookup"><span data-stu-id="51e37-122">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="51e37-123">forwardTo</span><span class="sxs-lookup"><span data-stu-id="51e37-123">forwardTo</span></span> | <span data-ttu-id="51e37-124">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="51e37-124">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="51e37-125">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada.</span><span class="sxs-lookup"><span data-stu-id="51e37-125">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="51e37-126">markAsRead</span><span class="sxs-lookup"><span data-stu-id="51e37-126">markAsRead</span></span> | <span data-ttu-id="51e37-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="51e37-127">Boolean</span></span> | <span data-ttu-id="51e37-128">Indica se uma mensagem deve ser marcada como lida.</span><span class="sxs-lookup"><span data-stu-id="51e37-128">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="51e37-129">markImportance</span><span class="sxs-lookup"><span data-stu-id="51e37-129">markImportance</span></span> | <span data-ttu-id="51e37-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e37-130">String</span></span> | <span data-ttu-id="51e37-131">Define a importância da mensagem, que pode ser: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="51e37-131">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="51e37-132">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="51e37-132">moveToFolder</span></span> |  <span data-ttu-id="51e37-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e37-133">String</span></span>| <span data-ttu-id="51e37-134">O ID da pasta para a qual uma mensagem será movida.</span><span class="sxs-lookup"><span data-stu-id="51e37-134">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="51e37-135">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="51e37-135">permanentDelete</span></span> | <span data-ttu-id="51e37-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="51e37-136">Boolean</span></span> | <span data-ttu-id="51e37-137">Indica se uma mensagem deve ser excluída permanentemente e não salva na pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="51e37-137">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="51e37-138">redirectTo</span><span class="sxs-lookup"><span data-stu-id="51e37-138">redirectTo</span></span> | [<span data-ttu-id="51e37-139">recipient</span><span class="sxs-lookup"><span data-stu-id="51e37-139">recipient</span></span>](recipient.md) | <span data-ttu-id="51e37-140">Os endereço de email para o qual uma mensagem deve ser redirecionada.</span><span class="sxs-lookup"><span data-stu-id="51e37-140">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="51e37-141">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="51e37-141">stopProcessingRules</span></span> | <span data-ttu-id="51e37-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="51e37-142">Boolean</span></span> | <span data-ttu-id="51e37-143">Indica se regras subsequentes devem ser avaliadas.</span><span class="sxs-lookup"><span data-stu-id="51e37-143">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="51e37-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51e37-144">JSON representation</span></span>
<span data-ttu-id="51e37-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51e37-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
