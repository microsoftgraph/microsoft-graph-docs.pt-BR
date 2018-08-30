# <a name="locationconstraint-resource-type"></a><span data-ttu-id="5d8ac-101">Tipo de recurso locationConstraint</span><span class="sxs-lookup"><span data-stu-id="5d8ac-101">locationConstraint resource type</span></span>

<span data-ttu-id="5d8ac-102">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="5d8ac-102">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d8ac-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d8ac-103">JSON representation</span></span>

<span data-ttu-id="5d8ac-104">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5d8ac-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="5d8ac-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d8ac-105">Properties</span></span>
| <span data-ttu-id="5d8ac-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d8ac-106">Property</span></span>     | <span data-ttu-id="5d8ac-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d8ac-107">Type</span></span>   |<span data-ttu-id="5d8ac-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d8ac-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d8ac-109">isRequired</span><span class="sxs-lookup"><span data-stu-id="5d8ac-109">isRequired</span></span>|<span data-ttu-id="5d8ac-110">Booleano</span><span class="sxs-lookup"><span data-stu-id="5d8ac-110">Boolean</span></span>|<span data-ttu-id="5d8ac-p101">O cliente solicita o serviço para incluir na resposta um local para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, [findMeetingTimes](../api/user_findmeetingtimes.md) não retorna nenhuma sugestão de horário para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, **findMeetingTimes** continuará procurando horários para a reunião sem local.</span><span class="sxs-lookup"><span data-stu-id="5d8ac-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user_findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="5d8ac-114">locations</span><span class="sxs-lookup"><span data-stu-id="5d8ac-114">locations</span></span>|<span data-ttu-id="5d8ac-115">Coleção [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="5d8ac-115">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="5d8ac-116">Informações de restrição de um ou mais locais que o cliente solicita para a reunião.</span><span class="sxs-lookup"><span data-stu-id="5d8ac-116">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="5d8ac-117">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="5d8ac-117">suggestLocation</span></span>|<span data-ttu-id="5d8ac-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="5d8ac-118">Boolean</span></span>|<span data-ttu-id="5d8ac-119">O cliente solicita o serviço para sugerir um ou mais locais para a reunião.</span><span class="sxs-lookup"><span data-stu-id="5d8ac-119">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->