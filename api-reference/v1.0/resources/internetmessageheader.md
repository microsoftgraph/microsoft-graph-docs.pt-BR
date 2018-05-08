# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="b6904-101">Tipo de recurso internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="b6904-101">internetMessageHeader resource type</span></span>


<span data-ttu-id="b6904-102">Um par chave-valor que representa um cabeçalho de mensagem da Internet, conforme definido pelo [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), que fornece detalhes do caminho de rede obtido por uma mensagem do remetente para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="b6904-102">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="b6904-103">Confira exemplos de um cabeçalho de mensagem da Internet em [Exibir cabeçalhos de mensagens de email](https://support.office.com/pt-BR/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="b6904-103">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/pt-BR/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="b6904-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6904-104">Properties</span></span>
| <span data-ttu-id="b6904-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6904-105">Property</span></span>     | <span data-ttu-id="b6904-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6904-106">Type</span></span>   |<span data-ttu-id="b6904-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6904-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6904-108">name</span><span class="sxs-lookup"><span data-stu-id="b6904-108">name</span></span>|<span data-ttu-id="b6904-109">string</span><span class="sxs-lookup"><span data-stu-id="b6904-109">string</span></span>|<span data-ttu-id="b6904-110">Representa a chave em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="b6904-110">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="b6904-111">valor</span><span class="sxs-lookup"><span data-stu-id="b6904-111">value</span></span>|<span data-ttu-id="b6904-112">string</span><span class="sxs-lookup"><span data-stu-id="b6904-112">string</span></span>|<span data-ttu-id="b6904-113">O valor em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="b6904-113">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6904-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6904-114">JSON representation</span></span>

<span data-ttu-id="b6904-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6904-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->