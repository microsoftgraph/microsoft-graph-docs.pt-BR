---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 8b39f20830da6621b1b6379674d5ef191afe5d9f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341015"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="086ad-102">Tipo de recurso CurrencyColumn</span><span class="sxs-lookup"><span data-stu-id="086ad-102">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="086ad-103">**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.</span><span class="sxs-lookup"><span data-stu-id="086ad-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="086ad-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="086ad-104">JSON representation</span></span>

<span data-ttu-id="086ad-105">Aqui está uma representação JSON de um recurso **currencyColumn**.</span><span class="sxs-lookup"><span data-stu-id="086ad-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="086ad-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="086ad-106">Properties</span></span>

| <span data-ttu-id="086ad-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="086ad-107">Property name</span></span> | <span data-ttu-id="086ad-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="086ad-108">Type</span></span>   | <span data-ttu-id="086ad-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="086ad-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="086ad-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="086ad-110">**locale**</span></span>    | <span data-ttu-id="086ad-111">string</span><span class="sxs-lookup"><span data-stu-id="086ad-111">string</span></span> | <span data-ttu-id="086ad-112">Especifica a localidade da qual o símbolo de moeda deverá ser inferido.</span><span class="sxs-lookup"><span data-stu-id="086ad-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": []
}
-->
