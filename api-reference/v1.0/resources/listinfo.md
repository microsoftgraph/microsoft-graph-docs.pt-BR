---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 459e51af92e01d10edd2ec1d86f3c288b125e1d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957463"
---
# <a name="listinfo-resource"></a><span data-ttu-id="170c6-102">Recurso de ListInfo</span><span class="sxs-lookup"><span data-stu-id="170c6-102">ListInfo resource</span></span>

<span data-ttu-id="170c6-103">O tipo complexo **listInfo** oferece informações adicionais sobre uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="170c6-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[lista]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="170c6-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="170c6-105">JSON representation</span></span>

<span data-ttu-id="170c6-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="170c6-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="170c6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="170c6-107">Properties</span></span>

| <span data-ttu-id="170c6-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="170c6-108">Property name</span></span>           | <span data-ttu-id="170c6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="170c6-109">Type</span></span>    | <span data-ttu-id="170c6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="170c6-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="170c6-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="170c6-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="170c6-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="170c6-112">Boolean</span></span> | <span data-ttu-id="170c6-113">Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="170c6-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="170c6-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="170c6-114">**hidden**</span></span>              | <span data-ttu-id="170c6-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="170c6-115">Boolean</span></span> | <span data-ttu-id="170c6-116">Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="170c6-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="170c6-117">**template**</span><span class="sxs-lookup"><span data-stu-id="170c6-117">**template**</span></span>            | <span data-ttu-id="170c6-118">String</span><span class="sxs-lookup"><span data-stu-id="170c6-118">String</span></span>  | <span data-ttu-id="170c6-119">Um valor enumerado que representa o modelo de lista básica usado na criação da lista.</span><span class="sxs-lookup"><span data-stu-id="170c6-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="170c6-120">Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.</span><span class="sxs-lookup"><span data-stu-id="170c6-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="170c6-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="170c6-121">Remarks</span></span>

<span data-ttu-id="170c6-122">Embora a maioria das listas criadas pelos usuários tenha um dos valores listados acima, outros valores também são possíveis.</span><span class="sxs-lookup"><span data-stu-id="170c6-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="170c6-123">Seu aplicativo deve estar preparado para lidar com os valores que não estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="170c6-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="170c6-124">Para os desenvolvedores familiarizados com APIs de CSOM do SharePoint, o valor `template` corresponde à enumeração `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="170c6-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

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
