---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7fb11fc9dc2f55b853ec512255ffa06f8a53cef6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933670"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="db25a-102">Recurso SiteCollection</span><span class="sxs-lookup"><span data-stu-id="db25a-102">SiteCollection resource</span></span>

> <span data-ttu-id="db25a-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="db25a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db25a-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="db25a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db25a-105">O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="db25a-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="db25a-106">Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="db25a-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db25a-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db25a-107">JSON representation</span></span>

<span data-ttu-id="db25a-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db25a-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="db25a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db25a-109">Properties</span></span>

| <span data-ttu-id="db25a-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="db25a-110">Property name</span></span>        | <span data-ttu-id="db25a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="db25a-111">Type</span></span>     | <span data-ttu-id="db25a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="db25a-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="db25a-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="db25a-113">**hostname**</span></span>         | <span data-ttu-id="db25a-114">string</span><span class="sxs-lookup"><span data-stu-id="db25a-114">string</span></span>   | <span data-ttu-id="db25a-p102">O nome do host do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db25a-p102">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="db25a-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="db25a-117">**dataLocationCode**</span></span> | <span data-ttu-id="db25a-118">string</span><span class="sxs-lookup"><span data-stu-id="db25a-118">string</span></span>   | <span data-ttu-id="db25a-119">O código de região geográfica para onde esse conjunto de sites reside.</span><span class="sxs-lookup"><span data-stu-id="db25a-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="db25a-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db25a-120">Read-only.</span></span>
| <span data-ttu-id="db25a-121">**root**</span><span class="sxs-lookup"><span data-stu-id="db25a-121">**root**</span></span>             | <span data-ttu-id="db25a-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="db25a-122">[root][]</span></span> | <span data-ttu-id="db25a-123">Se presente, indica que este é um conjunto de sites raiz no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="db25a-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="db25a-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db25a-124">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
