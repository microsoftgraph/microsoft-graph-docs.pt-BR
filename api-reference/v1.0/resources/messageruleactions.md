# <a name="messageruleactions-resource-type"></a><span data-ttu-id="db933-101">Tipo de recurso messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="db933-101">messageRuleActions resource type</span></span>


<span data-ttu-id="db933-102">Representa o conjunto de ações que estão disponíveis para uma regra.</span><span class="sxs-lookup"><span data-stu-id="db933-102">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="db933-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db933-103">Properties</span></span>
| <span data-ttu-id="db933-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db933-104">Property</span></span>     | <span data-ttu-id="db933-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="db933-105">Type</span></span>   |<span data-ttu-id="db933-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="db933-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db933-107">assignCategories</span><span class="sxs-lookup"><span data-stu-id="db933-107">assignCategories</span></span> | <span data-ttu-id="db933-108">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db933-108">String collection</span></span> | <span data-ttu-id="db933-109">Uma lista de categorias a serem atribuídas a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="db933-109">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="db933-110">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="db933-110">copyToFolder</span></span> | <span data-ttu-id="db933-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db933-111">String</span></span> | <span data-ttu-id="db933-112">O ID de uma pasta para a qual uma mensagem deve ser copiada.</span><span class="sxs-lookup"><span data-stu-id="db933-112">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="db933-113">delete</span><span class="sxs-lookup"><span data-stu-id="db933-113">delete</span></span> | <span data-ttu-id="db933-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="db933-114">Boolean</span></span> | <span data-ttu-id="db933-115">Indica se uma mensagem deve ser movida para a pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="db933-115">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="db933-116">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="db933-116">forwardAsAttachmentTo</span></span> | <span data-ttu-id="db933-117">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="db933-117">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="db933-118">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada como um anexo.</span><span class="sxs-lookup"><span data-stu-id="db933-118">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="db933-119">forwardTo</span><span class="sxs-lookup"><span data-stu-id="db933-119">forwardTo</span></span> | <span data-ttu-id="db933-120">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="db933-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="db933-121">Os endereços de email dos destinatários para os quais uma mensagem deve ser encaminhada.</span><span class="sxs-lookup"><span data-stu-id="db933-121">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="db933-122">markAsRead</span><span class="sxs-lookup"><span data-stu-id="db933-122">markAsRead</span></span> | <span data-ttu-id="db933-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="db933-123">Boolean</span></span> | <span data-ttu-id="db933-124">Indica se uma mensagem deve ser marcada como lida.</span><span class="sxs-lookup"><span data-stu-id="db933-124">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="db933-125">markImportance</span><span class="sxs-lookup"><span data-stu-id="db933-125">markImportance</span></span> | <span data-ttu-id="db933-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db933-126">String</span></span> | <span data-ttu-id="db933-127">Define a importância da mensagem, que pode ser: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="db933-127">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="db933-128">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="db933-128">moveToFolder</span></span> |  <span data-ttu-id="db933-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db933-129">String</span></span>| <span data-ttu-id="db933-130">O ID da pasta para a qual uma mensagem será movida.</span><span class="sxs-lookup"><span data-stu-id="db933-130">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="db933-131">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="db933-131">permanentDelete</span></span> | <span data-ttu-id="db933-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="db933-132">Boolean</span></span> | <span data-ttu-id="db933-133">Indica se uma mensagem deve ser excluída permanentemente e não salva na pasta Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="db933-133">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="db933-134">redirectTo</span><span class="sxs-lookup"><span data-stu-id="db933-134">redirectTo</span></span> | [<span data-ttu-id="db933-135">recipient</span><span class="sxs-lookup"><span data-stu-id="db933-135">recipient</span></span>](recipient.md) | <span data-ttu-id="db933-136">Os endereço de email para o qual uma mensagem deve ser redirecionada.</span><span class="sxs-lookup"><span data-stu-id="db933-136">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="db933-137">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="db933-137">stopProcessingRules</span></span> | <span data-ttu-id="db933-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="db933-138">Boolean</span></span> | <span data-ttu-id="db933-139">Indica se regras subsequentes devem ser avaliadas.</span><span class="sxs-lookup"><span data-stu-id="db933-139">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="db933-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db933-140">JSON representation</span></span>
<span data-ttu-id="db933-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db933-141">Here is a JSON representation of the resource.</span></span>

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