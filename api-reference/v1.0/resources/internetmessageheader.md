---
title: Tipo de recurso internetMessageHeader
description: 'Um par de chave / valor que representa um cabeçalho de mensagem da Internet, conforme definido pela RFC5322, que fornece '
ms.openlocfilehash: 44c3e33807f45420f79c8216b8381a19c062e411
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006459"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="0afc5-103">Tipo de recurso internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="0afc5-103">internetMessageHeader resource type</span></span>


<span data-ttu-id="0afc5-104">Um par chave-valor que representa um cabeçalho de mensagem da Internet, conforme definido pelo [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), que fornece detalhes do caminho de rede obtido por uma mensagem do remetente para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="0afc5-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="0afc5-105">Confira exemplos de um cabeçalho de mensagem da Internet em [Exibir cabeçalhos de mensagens de email](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="0afc5-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="0afc5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0afc5-106">Properties</span></span>
| <span data-ttu-id="0afc5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0afc5-107">Property</span></span>     | <span data-ttu-id="0afc5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0afc5-108">Type</span></span>   |<span data-ttu-id="0afc5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0afc5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0afc5-110">name</span><span class="sxs-lookup"><span data-stu-id="0afc5-110">name</span></span>|<span data-ttu-id="0afc5-111">string</span><span class="sxs-lookup"><span data-stu-id="0afc5-111">string</span></span>|<span data-ttu-id="0afc5-112">Representa a chave em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="0afc5-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="0afc5-113">valor</span><span class="sxs-lookup"><span data-stu-id="0afc5-113">value</span></span>|<span data-ttu-id="0afc5-114">string</span><span class="sxs-lookup"><span data-stu-id="0afc5-114">string</span></span>|<span data-ttu-id="0afc5-115">O valor em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="0afc5-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0afc5-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0afc5-116">JSON representation</span></span>

<span data-ttu-id="0afc5-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0afc5-117">Here is a JSON representation of the resource.</span></span>

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