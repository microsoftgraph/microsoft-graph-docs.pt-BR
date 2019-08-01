---
title: Tipo de recurso internetMessageHeader
description: 'Um par chave-valor que representa um cabeçalho de mensagem da Internet, conforme definido pelo RFC5322, que fornece '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 14d4cb88c79651bbba381206df7d5ff9b26db0bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030195"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="48a6e-103">Tipo de recurso internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="48a6e-103">internetMessageHeader resource type</span></span>


<span data-ttu-id="48a6e-104">Um par chave-valor que representa um cabeçalho de mensagem da Internet, conforme definido pelo [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), que fornece detalhes do caminho de rede obtido por uma mensagem do remetente para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="48a6e-104">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="48a6e-105">Confira exemplos de um cabeçalho de mensagem da Internet em [Exibir cabeçalhos de mensagens de email](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="48a6e-105">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="48a6e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48a6e-106">Properties</span></span>
| <span data-ttu-id="48a6e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48a6e-107">Property</span></span>     | <span data-ttu-id="48a6e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="48a6e-108">Type</span></span>   |<span data-ttu-id="48a6e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="48a6e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48a6e-110">name</span><span class="sxs-lookup"><span data-stu-id="48a6e-110">name</span></span>|<span data-ttu-id="48a6e-111">string</span><span class="sxs-lookup"><span data-stu-id="48a6e-111">string</span></span>|<span data-ttu-id="48a6e-112">Representa a chave em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="48a6e-112">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="48a6e-113">valor</span><span class="sxs-lookup"><span data-stu-id="48a6e-113">value</span></span>|<span data-ttu-id="48a6e-114">string</span><span class="sxs-lookup"><span data-stu-id="48a6e-114">string</span></span>|<span data-ttu-id="48a6e-115">O valor em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="48a6e-115">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48a6e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48a6e-116">JSON representation</span></span>

<span data-ttu-id="48a6e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48a6e-117">Here is a JSON representation of the resource.</span></span>

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
