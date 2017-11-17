---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
ms.openlocfilehash: eb4952c1a49c41dfae6683153753711158c70f01
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="listinfo-resource"></a><span data-ttu-id="61023-102">Recurso de ListInfo</span><span class="sxs-lookup"><span data-stu-id="61023-102">ListInfo resource</span></span>

<span data-ttu-id="61023-103">O tipo complexo **listInfo** oferece informações adicionais sobre uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="61023-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="61023-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61023-105">JSON representation</span></span>

<span data-ttu-id="61023-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61023-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="61023-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61023-107">Properties</span></span>

| <span data-ttu-id="61023-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="61023-108">Property name</span></span>           | <span data-ttu-id="61023-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="61023-109">Type</span></span>    | <span data-ttu-id="61023-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="61023-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="61023-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="61023-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="61023-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="61023-112">Boolean</span></span> | <span data-ttu-id="61023-113">Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="61023-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="61023-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="61023-114">**Hidden**</span></span>              | <span data-ttu-id="61023-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="61023-115">Boolean</span></span> | <span data-ttu-id="61023-116">Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="61023-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="61023-117">**template**</span><span class="sxs-lookup"><span data-stu-id="61023-117">**template**</span></span>            | <span data-ttu-id="61023-118">String</span><span class="sxs-lookup"><span data-stu-id="61023-118">String</span></span>  | <span data-ttu-id="61023-119">Um valor enumerado que representa o modelo de lista básica usado na criação da lista.</span><span class="sxs-lookup"><span data-stu-id="61023-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="61023-120">Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.</span><span class="sxs-lookup"><span data-stu-id="61023-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="61023-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="61023-121">Remarks</span></span>

<span data-ttu-id="61023-122">Embora a maioria das listas criadas pelos usuários tenha um dos valores listados acima, outros valores também são possíveis.</span><span class="sxs-lookup"><span data-stu-id="61023-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="61023-123">Seu aplicativo deve estar preparado para lidar com os valores que não estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="61023-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="61023-124">Para os desenvolvedores familiarizados com APIs de CSOM do SharePoint, o valor `template` corresponde à enumeração `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="61023-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
