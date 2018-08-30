---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
ms.openlocfilehash: da8398bbb87111648ea561e1799e062ed46b0ee6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270773"
---
# <a name="listinfo-resource"></a><span data-ttu-id="1bd8f-102">Recurso de ListInfo</span><span class="sxs-lookup"><span data-stu-id="1bd8f-102">ListInfo resource</span></span>

<span data-ttu-id="1bd8f-103">O tipo complexo **listInfo** oferece informações adicionais sobre uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="1bd8f-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[lista]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="1bd8f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bd8f-105">JSON representation</span></span>

<span data-ttu-id="1bd8f-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bd8f-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="1bd8f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bd8f-107">Properties</span></span>

| <span data-ttu-id="1bd8f-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1bd8f-108">Property name</span></span>           | <span data-ttu-id="1bd8f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bd8f-109">Type</span></span>    | <span data-ttu-id="1bd8f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bd8f-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="1bd8f-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="1bd8f-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="1bd8f-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bd8f-112">Boolean</span></span> | <span data-ttu-id="1bd8f-113">Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="1bd8f-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="1bd8f-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="1bd8f-114">**hidden**</span></span>              | <span data-ttu-id="1bd8f-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="1bd8f-115">Boolean</span></span> | <span data-ttu-id="1bd8f-116">Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1bd8f-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="1bd8f-117">**template**</span><span class="sxs-lookup"><span data-stu-id="1bd8f-117">**template**</span></span>            | <span data-ttu-id="1bd8f-118">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bd8f-118">String</span></span>  | <span data-ttu-id="1bd8f-119">Um valor enumerado que representa o modelo de lista básica usado na criação da lista.</span><span class="sxs-lookup"><span data-stu-id="1bd8f-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="1bd8f-120">Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.</span><span class="sxs-lookup"><span data-stu-id="1bd8f-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="1bd8f-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="1bd8f-121">Remarks</span></span>

<span data-ttu-id="1bd8f-122">Embora a maioria das listas criadas pelos usuários tenha um dos valores listados acima, outros valores também são possíveis.</span><span class="sxs-lookup"><span data-stu-id="1bd8f-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="1bd8f-123">Seu aplicativo deve estar preparado para lidar com os valores que não estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="1bd8f-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="1bd8f-124">Para os desenvolvedores familiarizados com APIs de CSOM do SharePoint, o valor `template` corresponde à enumeração `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="1bd8f-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

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
