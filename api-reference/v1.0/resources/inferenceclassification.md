# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="4b0b6-101">Tipo de recurso inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="4b0b6-101">inferenceClassification resource type</span></span>

<span data-ttu-id="4b0b6-102">Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário.</span><span class="sxs-lookup"><span data-stu-id="4b0b6-102">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="4b0b6-103">Para saber mais, consulte [Gerenciar a Caixa de Entrada Prioritária](manage_focused_inbox.md).</span><span class="sxs-lookup"><span data-stu-id="4b0b6-103">For more information, see [Manage Focused Inbox](manage_focused_inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="4b0b6-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="4b0b6-104">Methods</span></span>

| <span data-ttu-id="4b0b6-105">Método</span><span class="sxs-lookup"><span data-stu-id="4b0b6-105">Method</span></span>           | <span data-ttu-id="4b0b6-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4b0b6-106">Return Type</span></span>    |<span data-ttu-id="4b0b6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b0b6-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4b0b6-108">Criar inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4b0b6-108">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification_post_overrides.md) |[<span data-ttu-id="4b0b6-109">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4b0b6-109">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="4b0b6-p101">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="4b0b6-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="4b0b6-112">Listar substituições</span><span class="sxs-lookup"><span data-stu-id="4b0b6-112">List overrides</span></span>](../api/inferenceclassification_list_overrides.md) |<span data-ttu-id="4b0b6-113">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="4b0b6-113">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="4b0b6-114">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="4b0b6-114">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b0b6-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b0b6-115">Properties</span></span>
| <span data-ttu-id="4b0b6-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b0b6-116">Property</span></span>     | <span data-ttu-id="4b0b6-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b0b6-117">Type</span></span>   |<span data-ttu-id="4b0b6-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b0b6-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b0b6-119">id</span><span class="sxs-lookup"><span data-stu-id="4b0b6-119">id</span></span>|<span data-ttu-id="4b0b6-120">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b0b6-120">string</span></span>| <span data-ttu-id="4b0b6-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4b0b6-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b0b6-122">Relações</span><span class="sxs-lookup"><span data-stu-id="4b0b6-122">Relationships</span></span>
| <span data-ttu-id="4b0b6-123">Relação</span><span class="sxs-lookup"><span data-stu-id="4b0b6-123">Relationship</span></span> | <span data-ttu-id="4b0b6-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b0b6-124">Type</span></span>   |<span data-ttu-id="4b0b6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b0b6-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b0b6-126">overrides</span><span class="sxs-lookup"><span data-stu-id="4b0b6-126">overrides</span></span>|<span data-ttu-id="4b0b6-127">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="4b0b6-127">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="4b0b6-p102">Um conjunto de substituições para um usuário sempre classificar mensagens a partir de remetentes específicos, de maneiras específicas: `focused`, ou `other`. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="4b0b6-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b0b6-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b0b6-131">JSON representation</span></span>

<span data-ttu-id="4b0b6-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b0b6-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->