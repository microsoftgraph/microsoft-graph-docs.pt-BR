---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
description: O tipo complexo listInfo oferece informações adicionais sobre uma lista.
doc_type: resourcePageType
ms.openlocfilehash: dd6b2d892746c5aafc599b988113aefaa0b9973d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036411"
---
# <a name="listinfo-resource"></a><span data-ttu-id="7b20f-103">Recurso de ListInfo</span><span class="sxs-lookup"><span data-stu-id="7b20f-103">ListInfo resource</span></span>

<span data-ttu-id="7b20f-104">O tipo complexo **listInfo** oferece informações adicionais sobre uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="7b20f-104">The **listInfo** complex type provides additional information about a [list][].</span></span>

[lista]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="7b20f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b20f-106">JSON representation</span></span>

<span data-ttu-id="7b20f-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b20f-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7b20f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b20f-108">Properties</span></span>

| <span data-ttu-id="7b20f-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7b20f-109">Property name</span></span>           | <span data-ttu-id="7b20f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b20f-110">Type</span></span>    | <span data-ttu-id="7b20f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b20f-111">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="7b20f-112">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="7b20f-112">**contentTypesEnabled**</span></span> | <span data-ttu-id="7b20f-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b20f-113">Boolean</span></span> | <span data-ttu-id="7b20f-114">Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="7b20f-114">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="7b20f-115">**hidden**</span><span class="sxs-lookup"><span data-stu-id="7b20f-115">**hidden**</span></span>              | <span data-ttu-id="7b20f-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b20f-116">Boolean</span></span> | <span data-ttu-id="7b20f-117">Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7b20f-117">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="7b20f-118">**template**</span><span class="sxs-lookup"><span data-stu-id="7b20f-118">**template**</span></span>            | <span data-ttu-id="7b20f-119">String</span><span class="sxs-lookup"><span data-stu-id="7b20f-119">String</span></span>  | <span data-ttu-id="7b20f-120">Um valor enumerado que representa o modelo de lista básica usado na criação da lista.</span><span class="sxs-lookup"><span data-stu-id="7b20f-120">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="7b20f-121">Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.</span><span class="sxs-lookup"><span data-stu-id="7b20f-121">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="7b20f-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="7b20f-122">Remarks</span></span>

<span data-ttu-id="7b20f-123">Embora a maioria das listas criadas pelos usuários tenha um dos valores listados acima, outros valores também são possíveis.</span><span class="sxs-lookup"><span data-stu-id="7b20f-123">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="7b20f-124">Seu aplicativo deve estar preparado para lidar com os valores que não estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="7b20f-124">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="7b20f-125">Para os desenvolvedores familiarizados com APIs de CSOM do SharePoint, o valor `template` corresponde à enumeração `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="7b20f-125">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

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
