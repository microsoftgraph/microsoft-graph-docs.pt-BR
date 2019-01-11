---
title: Tipo de recurso internetMessageHeader
description: 'Um par de chave / valor que representa um cabeçalho de mensagem da Internet, conforme definido pela RFC5322, que fornece '
localization_priority: Normal
ms.openlocfilehash: 2a8dd616ffe8417a5064c0a98976d512b1279704
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892348"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="9cb39-103">Tipo de recurso internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="9cb39-103">internetMessageHeader resource type</span></span>


<span data-ttu-id="9cb39-104">Um par chave-valor que representa um cabeçalho de mensagem da Internet, conforme definido pelo [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), que fornece detalhes do caminho de rede obtido por uma mensagem do remetente para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="9cb39-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="9cb39-105">Confira exemplos de um cabeçalho de mensagem da Internet em [Exibir cabeçalhos de mensagens de email](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="9cb39-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="9cb39-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cb39-106">Properties</span></span>
| <span data-ttu-id="9cb39-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cb39-107">Property</span></span>     | <span data-ttu-id="9cb39-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cb39-108">Type</span></span>   |<span data-ttu-id="9cb39-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cb39-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cb39-110">name</span><span class="sxs-lookup"><span data-stu-id="9cb39-110">name</span></span>|<span data-ttu-id="9cb39-111">string</span><span class="sxs-lookup"><span data-stu-id="9cb39-111">string</span></span>|<span data-ttu-id="9cb39-112">Representa a chave em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="9cb39-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="9cb39-113">valor</span><span class="sxs-lookup"><span data-stu-id="9cb39-113">value</span></span>|<span data-ttu-id="9cb39-114">string</span><span class="sxs-lookup"><span data-stu-id="9cb39-114">string</span></span>|<span data-ttu-id="9cb39-115">O valor em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="9cb39-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cb39-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cb39-116">JSON representation</span></span>

<span data-ttu-id="9cb39-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9cb39-117">Here is a JSON representation of the resource.</span></span>

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
