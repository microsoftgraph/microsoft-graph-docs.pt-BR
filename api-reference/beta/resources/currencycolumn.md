---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 179c0bb1e5c82d7f2af17dcbcae08be8726f2ecd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888932"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="cbbf7-102">Tipo de recurso CurrencyColumn</span><span class="sxs-lookup"><span data-stu-id="cbbf7-102">CurrencyColumn resource type</span></span>

> <span data-ttu-id="cbbf7-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cbbf7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbbf7-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cbbf7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbbf7-105">**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.</span><span class="sxs-lookup"><span data-stu-id="cbbf7-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbbf7-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbbf7-106">JSON representation</span></span>

<span data-ttu-id="cbbf7-107">Aqui está uma representação JSON de um recurso **currencyColumn**.</span><span class="sxs-lookup"><span data-stu-id="cbbf7-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="cbbf7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbbf7-108">Properties</span></span>

| <span data-ttu-id="cbbf7-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="cbbf7-109">Property name</span></span> | <span data-ttu-id="cbbf7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbbf7-110">Type</span></span>   | <span data-ttu-id="cbbf7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbbf7-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="cbbf7-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="cbbf7-112">**locale**</span></span>    | <span data-ttu-id="cbbf7-113">string</span><span class="sxs-lookup"><span data-stu-id="cbbf7-113">string</span></span> | <span data-ttu-id="cbbf7-114">Especifica a localidade da qual o símbolo de moeda deverá ser inferido.</span><span class="sxs-lookup"><span data-stu-id="cbbf7-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
