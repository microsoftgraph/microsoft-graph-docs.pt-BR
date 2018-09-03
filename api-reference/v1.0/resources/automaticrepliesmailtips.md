# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="475c4-101">tipo de recurso de automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="475c4-101">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="475c4-102">[Dicas de e-mail](../resources/mailtips.md) sobre qualquer resposta automática configurada em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="475c4-102">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="475c4-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="475c4-103">Properties</span></span>
| <span data-ttu-id="475c4-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="475c4-104">Property</span></span>     | <span data-ttu-id="475c4-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="475c4-105">Type</span></span>   |<span data-ttu-id="475c4-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="475c4-106">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="475c4-107">message</span><span class="sxs-lookup"><span data-stu-id="475c4-107">message</span></span> | <span data-ttu-id="475c4-108">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="475c4-108">String</span></span> | <span data-ttu-id="475c4-109">A mensagem de resposta automática.</span><span class="sxs-lookup"><span data-stu-id="475c4-109">The automatic reply message.</span></span> |
| <span data-ttu-id="475c4-110">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="475c4-110">messageLanguage</span></span> | [<span data-ttu-id="475c4-111">localeInfo</span><span class="sxs-lookup"><span data-stu-id="475c4-111">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="475c4-112">O idioma em que a mensagem de resposta automática está.</span><span class="sxs-lookup"><span data-stu-id="475c4-112">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="475c4-113">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="475c4-113">ScheduledEndTime</span></span> | [<span data-ttu-id="475c4-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="475c4-114">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="475c4-115">A data e a hora em que as respostas automáticas estão definidas para terminar.</span><span class="sxs-lookup"><span data-stu-id="475c4-115">The date and time that automatic replies are set to end, if Status is set to .</span></span> |
| <span data-ttu-id="475c4-116">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="475c4-116">ScheduledStartTime</span></span> | [<span data-ttu-id="475c4-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="475c4-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="475c4-118">A data e a hora em que as respostas automáticas são definidas para começar.</span><span class="sxs-lookup"><span data-stu-id="475c4-118">The date and time that automatic replies are set to begin, if Status is set to .</span></span> |

## <a name="json-representation"></a><span data-ttu-id="475c4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="475c4-119">JSON representation</span></span>

<span data-ttu-id="475c4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="475c4-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->