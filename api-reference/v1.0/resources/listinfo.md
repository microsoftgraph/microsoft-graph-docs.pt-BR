---
author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
description: O tipo complexo listInfo oferece informações adicionais sobre uma lista.
doc_type: resourcePageType
ms.openlocfilehash: c5d84f5fae89e6ecf433dad20a959f9846f58006
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239356"
---
# <a name="listinfo-resource"></a><span data-ttu-id="6719a-103">Recurso de ListInfo</span><span class="sxs-lookup"><span data-stu-id="6719a-103">ListInfo resource</span></span>

<span data-ttu-id="6719a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6719a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6719a-105">O tipo complexo **listInfo** oferece informações adicionais sobre uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="6719a-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[lista]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="6719a-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6719a-107">JSON representation</span></span>

<span data-ttu-id="6719a-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6719a-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a><span data-ttu-id="6719a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6719a-109">Properties</span></span>

| <span data-ttu-id="6719a-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6719a-110">Property name</span></span>           | <span data-ttu-id="6719a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6719a-111">Type</span></span>    | <span data-ttu-id="6719a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6719a-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="6719a-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="6719a-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="6719a-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="6719a-114">Boolean</span></span> | <span data-ttu-id="6719a-115">Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="6719a-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="6719a-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="6719a-116">**hidden**</span></span>              | <span data-ttu-id="6719a-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="6719a-117">Boolean</span></span> | <span data-ttu-id="6719a-118">Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6719a-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="6719a-119">**template**</span><span class="sxs-lookup"><span data-stu-id="6719a-119">**template**</span></span>            | <span data-ttu-id="6719a-120">String</span><span class="sxs-lookup"><span data-stu-id="6719a-120">String</span></span>  | <span data-ttu-id="6719a-121">Um valor enumerado que representa o modelo de lista básica usado na criação da lista.</span><span class="sxs-lookup"><span data-stu-id="6719a-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="6719a-122">Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.</span><span class="sxs-lookup"><span data-stu-id="6719a-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="6719a-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="6719a-123">Remarks</span></span>

<span data-ttu-id="6719a-124">Embora a maioria das listas criadas pelos usuários tenha um dos valores listados acima, outros valores também são possíveis.</span><span class="sxs-lookup"><span data-stu-id="6719a-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="6719a-125">Seu aplicativo deve estar preparado para lidar com os valores que não estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="6719a-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="6719a-126">Para os desenvolvedores familiarizados com APIs de CSOM do SharePoint, o valor `template` corresponde à enumeração `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="6719a-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/listinfo.md:
      Found potential enums in resource example that weren't defined in a table:(documentLibrary,genericList,tasks,survey,links,announcements,contacts,...) are in resource, but () are in table"
  ],
  "tocPath": ""
}-->

