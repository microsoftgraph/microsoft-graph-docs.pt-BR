# <a name="outlookitem-resource-type"></a><span data-ttu-id="44072-101">Tipo de recurso outlookItem</span><span class="sxs-lookup"><span data-stu-id="44072-101">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="44072-102">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44072-102">JSON representation</span></span>

<span data-ttu-id="44072-103">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="44072-103">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookItem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="44072-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44072-104">Properties</span></span>
| <span data-ttu-id="44072-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44072-105">Property</span></span>     | <span data-ttu-id="44072-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="44072-106">Type</span></span>   |<span data-ttu-id="44072-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="44072-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44072-108">categories</span><span class="sxs-lookup"><span data-stu-id="44072-108">categories</span></span>|<span data-ttu-id="44072-109">Conjunto de sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="44072-109">String collection</span></span>|<span data-ttu-id="44072-110">As categorias associadas ao item</span><span class="sxs-lookup"><span data-stu-id="44072-110">The categories associated with the message.</span></span>|
|<span data-ttu-id="44072-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="44072-111">changeKey</span></span>|<span data-ttu-id="44072-112">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="44072-112">String</span></span>|<span data-ttu-id="44072-113">Identifica a versão do item.</span><span class="sxs-lookup"><span data-stu-id="44072-113">Identifies the version of the contact.</span></span> <span data-ttu-id="44072-114">Toda vez que o item é alterado, changeKey também é alterado.</span><span class="sxs-lookup"><span data-stu-id="44072-114">Every time the contact is changed, ChangeKey  changes as well.</span></span> <span data-ttu-id="44072-115">Isso permite que o Exchange aplique alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="44072-115">Identifies the version of the reminder. Every time the reminder is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="44072-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44072-116">Read-only.</span></span>|
|<span data-ttu-id="44072-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44072-117">createdDateTime</span></span>|<span data-ttu-id="44072-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44072-118">DateTimeOffset</span></span>|<span data-ttu-id="44072-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="44072-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="44072-121">id</span><span class="sxs-lookup"><span data-stu-id="44072-121">id</span></span>|<span data-ttu-id="44072-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44072-122">String</span></span>| <span data-ttu-id="44072-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44072-123">Read-only.</span></span>|
|<span data-ttu-id="44072-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44072-124">lastModifiedDateTime</span></span>|<span data-ttu-id="44072-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44072-125">DateTimeOffset</span></span>|<span data-ttu-id="44072-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="44072-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="44072-128">Relações</span><span class="sxs-lookup"><span data-stu-id="44072-128">Relationships</span></span>
<span data-ttu-id="44072-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44072-129">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
