---
title: Tipo de recurso emailAddress
description: O nome e o endereço de email de um destinatário da mensagem ou contato.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3b6bddb5436408fa38c931cd7e1e1f5503979e5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032589"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="5bec4-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="5bec4-103">emailAddress resource type</span></span>

<span data-ttu-id="5bec4-104">O nome e o endereço de email de um destinatário da mensagem ou contato.</span><span class="sxs-lookup"><span data-stu-id="5bec4-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="5bec4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5bec4-105">Properties</span></span>
| <span data-ttu-id="5bec4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5bec4-106">Property</span></span>     | <span data-ttu-id="5bec4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5bec4-107">Type</span></span>   |<span data-ttu-id="5bec4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bec4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bec4-109">address</span><span class="sxs-lookup"><span data-stu-id="5bec4-109">address</span></span>|<span data-ttu-id="5bec4-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bec4-110">String</span></span>|<span data-ttu-id="5bec4-111">O endereço de email da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="5bec4-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="5bec4-112">name</span><span class="sxs-lookup"><span data-stu-id="5bec4-112">name</span></span>|<span data-ttu-id="5bec4-113">String</span><span class="sxs-lookup"><span data-stu-id="5bec4-113">String</span></span>|<span data-ttu-id="5bec4-114">O nome de exibição da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="5bec4-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bec4-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5bec4-115">JSON representation</span></span>

<span data-ttu-id="5bec4-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5bec4-116">Here is a JSON representation of the resource</span></span>

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
