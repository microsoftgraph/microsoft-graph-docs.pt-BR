<span data-ttu-id="0ec84-p102">Tipo de operação assíncrona. Os valores podem ser *ForceDelete* ou *Verification*</span><span class="sxs-lookup"><span data-stu-id="0ec84-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> | Tipo de operação assíncrona. Os valores podem ser *ForceDelete* ou *Verification* |
| <span data-ttu-id="0ec84-115">status</span><span class="sxs-lookup"><span data-stu-id="0ec84-115">status</span></span> | <span data-ttu-id="0ec84-116">String</span><span class="sxs-lookup"><span data-stu-id="0ec84-116">String</span></span> | <span data-ttu-id="0ec84-117">Status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="0ec84-117">Current status of the operation.</span></span> <br> <span data-ttu-id="0ec84-118">*Scheduled* – A operação foi agendada, mas não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="0ec84-118">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="0ec84-119">*InProgress* – A tarefa foi iniciada e está em andamento.</span><span class="sxs-lookup"><span data-stu-id="0ec84-119">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="0ec84-120">*Failed* - A operação falhou.</span><span class="sxs-lookup"><span data-stu-id="0ec84-120">*Failed* - Operation has failed.</span></span> |

## <span data-ttu-id="0ec84-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ec84-121">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="0ec84-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ec84-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->