---
title: Tipo de recurso internetMessageHeader
description: 'Um par chave-valor que representa um cabeçalho de mensagem da Internet, conforme definido pelo RFC5322, que fornece '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f717be91f466790c86b529d9cc81852e7c37853a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531258"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="067ff-103">Tipo de recurso internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="067ff-103">internetMessageHeader resource type</span></span>

<span data-ttu-id="067ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="067ff-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="067ff-105">Um par chave-valor que representa um cabeçalho de mensagem da Internet, conforme definido pelo [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), que fornece detalhes do caminho de rede obtido por uma mensagem do remetente para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="067ff-105">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="067ff-106">Confira exemplos de um cabeçalho de mensagem da Internet em [Exibir cabeçalhos de mensagens de email](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="067ff-106">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="067ff-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="067ff-107">Properties</span></span>
| <span data-ttu-id="067ff-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="067ff-108">Property</span></span>     | <span data-ttu-id="067ff-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="067ff-109">Type</span></span>   |<span data-ttu-id="067ff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="067ff-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="067ff-111">nome</span><span class="sxs-lookup"><span data-stu-id="067ff-111">name</span></span>|<span data-ttu-id="067ff-112">string</span><span class="sxs-lookup"><span data-stu-id="067ff-112">string</span></span>|<span data-ttu-id="067ff-113">Representa a chave em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="067ff-113">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="067ff-114">valor</span><span class="sxs-lookup"><span data-stu-id="067ff-114">value</span></span>|<span data-ttu-id="067ff-115">string</span><span class="sxs-lookup"><span data-stu-id="067ff-115">string</span></span>|<span data-ttu-id="067ff-116">O valor em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="067ff-116">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="067ff-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="067ff-117">JSON representation</span></span>

<span data-ttu-id="067ff-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="067ff-118">Here is a JSON representation of the resource.</span></span>

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
