---
title: Tipo de recurso emailAddress
description: O nome e o endereço de email de um destinatário da mensagem ou contato.
ms.openlocfilehash: 962b2f36af9e292125edc3da8606cd532b8c2ec0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003763"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="c3bf1-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="c3bf1-103">emailAddress resource type</span></span>

<span data-ttu-id="c3bf1-104">O nome e o endereço de email de um destinatário da mensagem ou contato.</span><span class="sxs-lookup"><span data-stu-id="c3bf1-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="c3bf1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3bf1-105">Properties</span></span>
| <span data-ttu-id="c3bf1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3bf1-106">Property</span></span>     | <span data-ttu-id="c3bf1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3bf1-107">Type</span></span>   |<span data-ttu-id="c3bf1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3bf1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3bf1-109">address</span><span class="sxs-lookup"><span data-stu-id="c3bf1-109">address</span></span>|<span data-ttu-id="c3bf1-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3bf1-110">String</span></span>|<span data-ttu-id="c3bf1-111">O endereço de email da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="c3bf1-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="c3bf1-112">name</span><span class="sxs-lookup"><span data-stu-id="c3bf1-112">name</span></span>|<span data-ttu-id="c3bf1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3bf1-113">String</span></span>|<span data-ttu-id="c3bf1-114">O nome de exibição da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="c3bf1-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3bf1-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3bf1-115">JSON representation</span></span>

<span data-ttu-id="c3bf1-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c3bf1-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
