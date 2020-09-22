---
title: tipo de recurso printUserIdentity
description: Representa uma identidade do usuário no serviço de impressão universal. Mapeia para um usuário do Azure AD.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8a695bed829d6c7e8825898da366737427195e1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070650"
---
# <a name="printuseridentity-resource-type"></a><span data-ttu-id="b1b5f-104">tipo de recurso printUserIdentity</span><span class="sxs-lookup"><span data-stu-id="b1b5f-104">printUserIdentity resource type</span></span>

<span data-ttu-id="b1b5f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1b5f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1b5f-106">Representa uma identidade do usuário no serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="b1b5f-106">Represents a user identity within the Universal Print service.</span></span> <span data-ttu-id="b1b5f-107">Mapeia para um [usuário do Azure Active Directory (Azure AD)](user.md).</span><span class="sxs-lookup"><span data-stu-id="b1b5f-107">Maps to an [Azure Active Directory (Azure AD) user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b1b5f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1b5f-108">Properties</span></span>
| <span data-ttu-id="b1b5f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1b5f-109">Property</span></span>     | <span data-ttu-id="b1b5f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1b5f-110">Type</span></span>        | <span data-ttu-id="b1b5f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1b5f-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1b5f-112">id</span><span class="sxs-lookup"><span data-stu-id="b1b5f-112">id</span></span>|<span data-ttu-id="b1b5f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1b5f-113">String</span></span>|<span data-ttu-id="b1b5f-114">O identificador do printUserIdentity.</span><span class="sxs-lookup"><span data-stu-id="b1b5f-114">The printUserIdentity's identifier.</span></span> <span data-ttu-id="b1b5f-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b1b5f-115">Read-only.</span></span>|
|<span data-ttu-id="b1b5f-116">displayName</span><span class="sxs-lookup"><span data-stu-id="b1b5f-116">displayName</span></span>|<span data-ttu-id="b1b5f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1b5f-117">String</span></span>|<span data-ttu-id="b1b5f-118">O nome de exibição do printUserIdentity.</span><span class="sxs-lookup"><span data-stu-id="b1b5f-118">The printUserIdentity's display name.</span></span>|
|<span data-ttu-id="b1b5f-119">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b1b5f-119">ipAddress</span></span>|<span data-ttu-id="b1b5f-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1b5f-120">String</span></span>|<span data-ttu-id="b1b5f-121">O endereço IP do printUserIdentity.</span><span class="sxs-lookup"><span data-stu-id="b1b5f-121">The printUserIdentity' IP address.</span></span> <span data-ttu-id="b1b5f-122">Não preenchido.</span><span class="sxs-lookup"><span data-stu-id="b1b5f-122">Not populated.</span></span>|
|<span data-ttu-id="b1b5f-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1b5f-123">userPrincipalName</span></span>|<span data-ttu-id="b1b5f-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1b5f-124">String</span></span>|<span data-ttu-id="b1b5f-125">O nome principal do usuário (UPN) do printUserIdentity.</span><span class="sxs-lookup"><span data-stu-id="b1b5f-125">The printUserIdentity's user principal name (UPN).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1b5f-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1b5f-126">JSON representation</span></span>

<span data-ttu-id="b1b5f-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1b5f-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUserIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUserIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


