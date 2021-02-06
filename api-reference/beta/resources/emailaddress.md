---
title: Tipo de recurso emailAddress
description: Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário da mensagem ou proprietário do calendário.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8f572058d50672a26b3930f90a7b0492f9aa1eca
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132556"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="fa18c-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="fa18c-103">emailAddress resource type</span></span>

<span data-ttu-id="fa18c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa18c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa18c-105">Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário da mensagem ou proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="fa18c-105">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="fa18c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa18c-106">Properties</span></span>
| <span data-ttu-id="fa18c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa18c-107">Property</span></span>     | <span data-ttu-id="fa18c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa18c-108">Type</span></span>   |<span data-ttu-id="fa18c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa18c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa18c-110">address</span><span class="sxs-lookup"><span data-stu-id="fa18c-110">address</span></span>|<span data-ttu-id="fa18c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa18c-111">String</span></span>|<span data-ttu-id="fa18c-112">O endereço de email de uma instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="fa18c-112">The email address of an entity instance.</span></span>|
|<span data-ttu-id="fa18c-113">nome</span><span class="sxs-lookup"><span data-stu-id="fa18c-113">name</span></span>|<span data-ttu-id="fa18c-114">String</span><span class="sxs-lookup"><span data-stu-id="fa18c-114">String</span></span>|<span data-ttu-id="fa18c-115">O nome de exibição de uma instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="fa18c-115">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa18c-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa18c-116">JSON representation</span></span>

<span data-ttu-id="fa18c-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fa18c-117">Here is a JSON representation of the resource</span></span>

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


