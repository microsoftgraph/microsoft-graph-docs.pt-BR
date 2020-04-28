---
title: tipo de recurso de multiidentity
description: Representa uma identidade no serviço de impressão universal. Mapeia para um grupo do Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: d4ac0695357aba0ba6c44fef4654d2edaefca6cb
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917597"
---
# <a name="printidentity-resource-type"></a><span data-ttu-id="2acf4-104">tipo de recurso de multiidentity</span><span class="sxs-lookup"><span data-stu-id="2acf4-104">printIdentity resource type</span></span>

<span data-ttu-id="2acf4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2acf4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2acf4-106">Representa uma identidade no serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="2acf4-106">Represents an identity within the Universal Print service.</span></span> <span data-ttu-id="2acf4-107">Mapeia para um [grupo do Azure Active Directory (Azure AD)](group.md).</span><span class="sxs-lookup"><span data-stu-id="2acf4-107">Maps to an [Azure Active Directory (Azure AD) group](group.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2acf4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2acf4-108">Properties</span></span>
| <span data-ttu-id="2acf4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2acf4-109">Property</span></span>     | <span data-ttu-id="2acf4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2acf4-110">Type</span></span>        | <span data-ttu-id="2acf4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2acf4-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2acf4-112">id</span><span class="sxs-lookup"><span data-stu-id="2acf4-112">id</span></span>|<span data-ttu-id="2acf4-113">String</span><span class="sxs-lookup"><span data-stu-id="2acf4-113">String</span></span>|<span data-ttu-id="2acf4-114">O identificador da multiidentity.</span><span class="sxs-lookup"><span data-stu-id="2acf4-114">The printIdentity's identifier.</span></span> <span data-ttu-id="2acf4-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2acf4-115">Read-only.</span></span>|
|<span data-ttu-id="2acf4-116">displayName</span><span class="sxs-lookup"><span data-stu-id="2acf4-116">displayName</span></span>|<span data-ttu-id="2acf4-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2acf4-117">String</span></span>|<span data-ttu-id="2acf4-118">O nome de exibição do multiidentity.</span><span class="sxs-lookup"><span data-stu-id="2acf4-118">The printIdentity's display name.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2acf4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2acf4-119">JSON representation</span></span>

<span data-ttu-id="2acf4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2acf4-120">The following is a JSON representation of the resource.</span></span>

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
