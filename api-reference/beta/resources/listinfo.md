---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1f94bf51169a6b056e010386f88d859aeaf41b9b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512371"
---
# <a name="listinfo-resource"></a><span data-ttu-id="de1a6-102">Recurso de ListInfo</span><span class="sxs-lookup"><span data-stu-id="de1a6-102">ListInfo resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de1a6-103">O tipo complexo **listInfo** oferece informações adicionais sobre uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="de1a6-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[lista]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="de1a6-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de1a6-105">JSON representation</span></span>

<span data-ttu-id="de1a6-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de1a6-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="de1a6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de1a6-107">Properties</span></span>

| <span data-ttu-id="de1a6-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="de1a6-108">Property name</span></span>           | <span data-ttu-id="de1a6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="de1a6-109">Type</span></span>    | <span data-ttu-id="de1a6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="de1a6-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="de1a6-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="de1a6-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="de1a6-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="de1a6-112">Boolean</span></span> | <span data-ttu-id="de1a6-113">Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="de1a6-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="de1a6-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="de1a6-114">**hidden**</span></span>              | <span data-ttu-id="de1a6-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="de1a6-115">Boolean</span></span> | <span data-ttu-id="de1a6-116">Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="de1a6-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="de1a6-117">**template**</span><span class="sxs-lookup"><span data-stu-id="de1a6-117">**template**</span></span>            | <span data-ttu-id="de1a6-118">String</span><span class="sxs-lookup"><span data-stu-id="de1a6-118">String</span></span>  | <span data-ttu-id="de1a6-119">Um valor enumerado que representa o modelo de lista básica usado na criação da lista.</span><span class="sxs-lookup"><span data-stu-id="de1a6-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="de1a6-120">Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.</span><span class="sxs-lookup"><span data-stu-id="de1a6-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="de1a6-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="de1a6-121">Remarks</span></span>

<span data-ttu-id="de1a6-122">Embora a maioria das listas criadas pelos usuários tenha um dos valores listados acima, outros valores também são possíveis.</span><span class="sxs-lookup"><span data-stu-id="de1a6-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="de1a6-123">Seu aplicativo deve estar preparado para lidar com os valores que não estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="de1a6-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="de1a6-124">Para os desenvolvedores familiarizados com APIs de CSOM do SharePoint, o valor `template` corresponde à enumeração `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="de1a6-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/listinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
