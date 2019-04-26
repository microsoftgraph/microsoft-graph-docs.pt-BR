---
title: Tipo de recurso emailAddress
description: O nome e o endereço de email de um destinatário da mensagem ou contato.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7af23418132c4d1c20097899f870c7d25be119bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555904"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="fdc16-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="fdc16-103">emailAddress resource type</span></span>

<span data-ttu-id="fdc16-104">O nome e o endereço de email de um destinatário da mensagem ou contato.</span><span class="sxs-lookup"><span data-stu-id="fdc16-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="fdc16-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdc16-105">Properties</span></span>
| <span data-ttu-id="fdc16-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdc16-106">Property</span></span>     | <span data-ttu-id="fdc16-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdc16-107">Type</span></span>   |<span data-ttu-id="fdc16-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdc16-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdc16-109">address</span><span class="sxs-lookup"><span data-stu-id="fdc16-109">address</span></span>|<span data-ttu-id="fdc16-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdc16-110">String</span></span>|<span data-ttu-id="fdc16-111">O endereço de email da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="fdc16-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="fdc16-112">name</span><span class="sxs-lookup"><span data-stu-id="fdc16-112">name</span></span>|<span data-ttu-id="fdc16-113">String</span><span class="sxs-lookup"><span data-stu-id="fdc16-113">String</span></span>|<span data-ttu-id="fdc16-114">O nome de exibição da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="fdc16-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdc16-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdc16-115">JSON representation</span></span>

<span data-ttu-id="fdc16-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fdc16-116">Here is a JSON representation of the resource</span></span>

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
