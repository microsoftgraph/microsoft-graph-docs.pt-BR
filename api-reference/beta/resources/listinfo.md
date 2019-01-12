---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0e1106873a9f069870c981f6df3ae94412ca85de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987766"
---
# <a name="listinfo-resource"></a><span data-ttu-id="ab17f-102">Recurso de ListInfo</span><span class="sxs-lookup"><span data-stu-id="ab17f-102">ListInfo resource</span></span>

> <span data-ttu-id="ab17f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab17f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab17f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab17f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab17f-105">O tipo complexo **listInfo** oferece informações adicionais sobre uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="ab17f-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[lista]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="ab17f-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab17f-107">JSON representation</span></span>

<span data-ttu-id="ab17f-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab17f-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ab17f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab17f-109">Properties</span></span>

| <span data-ttu-id="ab17f-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ab17f-110">Property name</span></span>           | <span data-ttu-id="ab17f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab17f-111">Type</span></span>    | <span data-ttu-id="ab17f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab17f-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="ab17f-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="ab17f-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="ab17f-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab17f-114">Boolean</span></span> | <span data-ttu-id="ab17f-115">Se `true`, indica que os tipos de conteúdo estão habilitados nesta lista.</span><span class="sxs-lookup"><span data-stu-id="ab17f-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="ab17f-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="ab17f-116">**hidden**</span></span>              | <span data-ttu-id="ab17f-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="ab17f-117">Boolean</span></span> | <span data-ttu-id="ab17f-118">Se `true`, indica que a lista não fica visível normalmente na experiência de usuário do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ab17f-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="ab17f-119">**template**</span><span class="sxs-lookup"><span data-stu-id="ab17f-119">**template**</span></span>            | <span data-ttu-id="ab17f-120">String</span><span class="sxs-lookup"><span data-stu-id="ab17f-120">String</span></span>  | <span data-ttu-id="ab17f-121">Um valor enumerado que representa o modelo de lista básica usado na criação da lista.</span><span class="sxs-lookup"><span data-stu-id="ab17f-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="ab17f-122">Os valores possíveis incluem `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` e mais.</span><span class="sxs-lookup"><span data-stu-id="ab17f-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="ab17f-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="ab17f-123">Remarks</span></span>

<span data-ttu-id="ab17f-124">Embora a maioria das listas criadas pelos usuários tenha um dos valores listados acima, outros valores também são possíveis.</span><span class="sxs-lookup"><span data-stu-id="ab17f-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="ab17f-125">Seu aplicativo deve estar preparado para lidar com os valores que não estão listados aqui.</span><span class="sxs-lookup"><span data-stu-id="ab17f-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="ab17f-126">Para os desenvolvedores familiarizados com APIs de CSOM do SharePoint, o valor `template` corresponde à enumeração `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="ab17f-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
