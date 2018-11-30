---
title: Tipo de recurso internetMessageHeader
description: 'Um par de chave / valor que representa um cabeçalho de mensagem da Internet, conforme definido pela RFC5322, que fornece '
ms.openlocfilehash: 420d39b6a139563e3f5f277f032f0f7a29252337
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036242"
---
# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="dd4d9-103">Tipo de recurso internetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="dd4d9-103">internetMessageHeader resource type</span></span>

> <span data-ttu-id="dd4d9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd4d9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd4d9-106">Um par chave-valor que representa um cabeçalho de mensagem da Internet, conforme definido pelo [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), que fornece detalhes do caminho de rede obtido por uma mensagem do remetente para o destinatário.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-106">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="dd4d9-107">Confira exemplos de um cabeçalho de mensagem da Internet em [Exibir cabeçalhos de mensagens de email](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span><span class="sxs-lookup"><span data-stu-id="dd4d9-107">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="dd4d9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd4d9-108">Properties</span></span>
| <span data-ttu-id="dd4d9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd4d9-109">Property</span></span>     | <span data-ttu-id="dd4d9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd4d9-110">Type</span></span>   |<span data-ttu-id="dd4d9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd4d9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd4d9-112">name</span><span class="sxs-lookup"><span data-stu-id="dd4d9-112">name</span></span>|<span data-ttu-id="dd4d9-113">string</span><span class="sxs-lookup"><span data-stu-id="dd4d9-113">string</span></span>|<span data-ttu-id="dd4d9-114">Representa a chave em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-114">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="dd4d9-115">valor</span><span class="sxs-lookup"><span data-stu-id="dd4d9-115">value</span></span>|<span data-ttu-id="dd4d9-116">string</span><span class="sxs-lookup"><span data-stu-id="dd4d9-116">string</span></span>|<span data-ttu-id="dd4d9-117">O valor em um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-117">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd4d9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd4d9-118">JSON representation</span></span>

<span data-ttu-id="dd4d9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-119">Here is a JSON representation of the resource.</span></span>

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