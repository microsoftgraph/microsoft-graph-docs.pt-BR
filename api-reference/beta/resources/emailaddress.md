---
title: Tipo de recurso emailAddress
description: Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário de mensagem ou proprietário do calendário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e0df635fb930816fa29b0d7f75a2075759a4c54d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499558"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="db734-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="db734-103">emailAddress resource type</span></span>

<span data-ttu-id="db734-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db734-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db734-105">Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário de mensagem ou proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="db734-105">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="db734-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db734-106">Properties</span></span>
| <span data-ttu-id="db734-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db734-107">Property</span></span>     | <span data-ttu-id="db734-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="db734-108">Type</span></span>   |<span data-ttu-id="db734-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="db734-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db734-110">address</span><span class="sxs-lookup"><span data-stu-id="db734-110">address</span></span>|<span data-ttu-id="db734-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db734-111">String</span></span>|<span data-ttu-id="db734-112">O endereço de email de uma instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="db734-112">The email address of an entity instance.</span></span>|
|<span data-ttu-id="db734-113">nome</span><span class="sxs-lookup"><span data-stu-id="db734-113">name</span></span>|<span data-ttu-id="db734-114">String</span><span class="sxs-lookup"><span data-stu-id="db734-114">String</span></span>|<span data-ttu-id="db734-115">O nome de exibição de uma instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="db734-115">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db734-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db734-116">JSON representation</span></span>

<span data-ttu-id="db734-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="db734-117">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
