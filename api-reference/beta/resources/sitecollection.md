---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.openlocfilehash: a0c55967ed7f7a397e0c8c0a4ce607921dc8a9f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830545"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="decee-102">Recurso SiteCollection</span><span class="sxs-lookup"><span data-stu-id="decee-102">SiteCollection resource</span></span>

> <span data-ttu-id="decee-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="decee-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="decee-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="decee-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="decee-105">O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="decee-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="decee-106">Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="decee-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="decee-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="decee-107">JSON representation</span></span>

<span data-ttu-id="decee-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="decee-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="decee-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="decee-109">Properties</span></span>

| <span data-ttu-id="decee-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="decee-110">Property name</span></span>        | <span data-ttu-id="decee-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="decee-111">Type</span></span>     | <span data-ttu-id="decee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="decee-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="decee-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="decee-113">**hostname**</span></span>         | <span data-ttu-id="decee-114">string</span><span class="sxs-lookup"><span data-stu-id="decee-114">string</span></span>   | <span data-ttu-id="decee-p102">O nome do host do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="decee-p102">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="decee-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="decee-117">**dataLocationCode**</span></span> | <span data-ttu-id="decee-118">string</span><span class="sxs-lookup"><span data-stu-id="decee-118">string</span></span>   | <span data-ttu-id="decee-119">O código de região geográfica para onde esse conjunto de sites reside.</span><span class="sxs-lookup"><span data-stu-id="decee-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="decee-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="decee-120">Read-only.</span></span>
| <span data-ttu-id="decee-121">**root**</span><span class="sxs-lookup"><span data-stu-id="decee-121">**root**</span></span>             | <span data-ttu-id="decee-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="decee-122">[root][]</span></span> | <span data-ttu-id="decee-123">Se presente, indica que este é um conjunto de sites raiz no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="decee-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="decee-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="decee-124">Read-only.</span></span>

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
