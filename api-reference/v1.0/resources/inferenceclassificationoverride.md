# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="4673e-101">Tipo de recurso inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4673e-101">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="4673e-102">Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.</span><span class="sxs-lookup"><span data-stu-id="4673e-102">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="4673e-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="4673e-103">Methods</span></span>

| <span data-ttu-id="4673e-104">Método</span><span class="sxs-lookup"><span data-stu-id="4673e-104">Method</span></span>           | <span data-ttu-id="4673e-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4673e-105">Return Type</span></span>    |<span data-ttu-id="4673e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="4673e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4673e-107">Atualizar</span><span class="sxs-lookup"><span data-stu-id="4673e-107">Update</span></span>](../api/inferenceclassificationoverride_update.md) | [<span data-ttu-id="4673e-108">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4673e-108">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="4673e-109">Altere o campo **ClassifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="4673e-109">Change the **classifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="4673e-110">Excluir</span><span class="sxs-lookup"><span data-stu-id="4673e-110">Delete</span></span>](../api/inferenceclassificationoverride_delete.md) | <span data-ttu-id="4673e-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4673e-111">None</span></span> |<span data-ttu-id="4673e-112">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="4673e-112">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="4673e-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4673e-113">Properties</span></span>
| <span data-ttu-id="4673e-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4673e-114">Property</span></span>     | <span data-ttu-id="4673e-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="4673e-115">Type</span></span>   |<span data-ttu-id="4673e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="4673e-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4673e-117">classifyAs</span><span class="sxs-lookup"><span data-stu-id="4673e-117">classifyAs</span></span>|<span data-ttu-id="4673e-118">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="4673e-118">InferenceClassificationType</span></span>| <span data-ttu-id="4673e-119">Especifica como as mensagens recebidas de um remetente específico sempre devem ser classificadas.</span><span class="sxs-lookup"><span data-stu-id="4673e-119">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: , .</span></span> <span data-ttu-id="4673e-120">Os valores possíveis são: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="4673e-120">The possible values are:</span></span>|
|<span data-ttu-id="4673e-121">id</span><span class="sxs-lookup"><span data-stu-id="4673e-121">id</span></span>|<span data-ttu-id="4673e-122">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="4673e-122">string</span></span>| <span data-ttu-id="4673e-p102">O identificador exclusivo da substituição. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4673e-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="4673e-125">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="4673e-125">senderEmailAddress</span></span>|[<span data-ttu-id="4673e-126">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4673e-126">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="4673e-127">A informação de endereço de email do remetente para quem a substituição é criada.</span><span class="sxs-lookup"><span data-stu-id="4673e-127">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4673e-128">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="4673e-128">Relationships</span></span>
<span data-ttu-id="4673e-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4673e-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4673e-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4673e-130">JSON representation</span></span>

<span data-ttu-id="4673e-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4673e-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->