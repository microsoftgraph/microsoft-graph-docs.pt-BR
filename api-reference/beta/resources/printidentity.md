---
title: tipo de recurso de multiidentity
description: Representa uma identidade no serviço de impressão universal. Mapeia para um grupo do Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 45a69cbad25d2f9c3c99c9e01aa47982fe5c62b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048761"
---
# <a name="printidentity-resource-type"></a><span data-ttu-id="ab45f-104">tipo de recurso de multiidentity</span><span class="sxs-lookup"><span data-stu-id="ab45f-104">printIdentity resource type</span></span>

<span data-ttu-id="ab45f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab45f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab45f-106">Representa uma identidade no serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="ab45f-106">Represents an identity within the Universal Print service.</span></span> <span data-ttu-id="ab45f-107">Mapeia para um [grupo do Azure Active Directory (Azure AD)](group.md).</span><span class="sxs-lookup"><span data-stu-id="ab45f-107">Maps to an [Azure Active Directory (Azure AD) group](group.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ab45f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab45f-108">Properties</span></span>
| <span data-ttu-id="ab45f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab45f-109">Property</span></span>     | <span data-ttu-id="ab45f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab45f-110">Type</span></span>        | <span data-ttu-id="ab45f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab45f-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ab45f-112">id</span><span class="sxs-lookup"><span data-stu-id="ab45f-112">id</span></span>|<span data-ttu-id="ab45f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab45f-113">String</span></span>|<span data-ttu-id="ab45f-114">O identificador da multiidentity.</span><span class="sxs-lookup"><span data-stu-id="ab45f-114">The printIdentity's identifier.</span></span> <span data-ttu-id="ab45f-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab45f-115">Read-only.</span></span>|
|<span data-ttu-id="ab45f-116">displayName</span><span class="sxs-lookup"><span data-stu-id="ab45f-116">displayName</span></span>|<span data-ttu-id="ab45f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab45f-117">String</span></span>|<span data-ttu-id="ab45f-118">O nome de exibição do multiidentity.</span><span class="sxs-lookup"><span data-stu-id="ab45f-118">The printIdentity's display name.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab45f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab45f-119">JSON representation</span></span>

<span data-ttu-id="ab45f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab45f-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


