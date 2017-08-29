# <a name="recipient-resource-type"></a><span data-ttu-id="6d144-101">Tipo de recurso recipient</span><span class="sxs-lookup"><span data-stu-id="6d144-101">recipient resource type</span></span>

<span data-ttu-id="6d144-102">Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="6d144-102">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="6d144-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d144-103">Properties</span></span>
| <span data-ttu-id="6d144-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d144-104">Property</span></span>     | <span data-ttu-id="6d144-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d144-105">Type</span></span>   |<span data-ttu-id="6d144-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d144-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d144-107">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6d144-107">emailAddress</span></span>|[<span data-ttu-id="6d144-108">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="6d144-108">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="6d144-109">O endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="6d144-109">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d144-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d144-110">JSON representation</span></span>

<span data-ttu-id="6d144-111">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6d144-111">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->