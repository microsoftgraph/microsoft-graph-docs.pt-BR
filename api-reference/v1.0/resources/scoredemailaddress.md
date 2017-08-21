# <a name="scoredemailaddress-resource-type"></a><span data-ttu-id="abfba-101">tipo de recurso scoredEmailAddress</span><span class="sxs-lookup"><span data-stu-id="abfba-101">scoredEmailAddress resource type</span></span>

<span data-ttu-id="abfba-102">Representa um endereço de email pontuado.</span><span class="sxs-lookup"><span data-stu-id="abfba-102">Represents a scored email address.</span></span>


## <a name="properties"></a><span data-ttu-id="abfba-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abfba-103">Properties</span></span>
| <span data-ttu-id="abfba-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abfba-104">Property</span></span>     | <span data-ttu-id="abfba-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="abfba-105">Type</span></span>   |<span data-ttu-id="abfba-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="abfba-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abfba-107">address</span><span class="sxs-lookup"><span data-stu-id="abfba-107">address</span></span>|<span data-ttu-id="abfba-108">string</span><span class="sxs-lookup"><span data-stu-id="abfba-108">string</span></span>|<span data-ttu-id="abfba-109">O endereço de email.</span><span class="sxs-lookup"><span data-stu-id="abfba-109">The recipient's email address.</span></span>|
|<span data-ttu-id="abfba-110">relevanceScore</span><span class="sxs-lookup"><span data-stu-id="abfba-110">relevanceScore</span></span>|<span data-ttu-id="abfba-111">duplo</span><span class="sxs-lookup"><span data-stu-id="abfba-111">double</span></span>|<span data-ttu-id="abfba-p101">A pontuação de relevância do endereço de email. Uma pontuação de relevância é usada como uma chave de classificação em relação aos outros resultados retornados. Um valor mais alto de pontuação de relevância corresponde a um resultado mais relevante. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="abfba-p101">The relevance score of the email address. A relevance score is used as a sort key, in relation to the other returned results. A higher relevance score value corresponds to a more relevant result. Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="abfba-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abfba-116">JSON representation</span></span>

<span data-ttu-id="abfba-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abfba-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
