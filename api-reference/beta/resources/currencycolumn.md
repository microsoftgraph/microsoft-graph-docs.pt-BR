---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
ms.openlocfilehash: 21c95026eb61eb68c98010d8ac288be115e95ec8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040854"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="6e48d-102">Tipo de recurso CurrencyColumn</span><span class="sxs-lookup"><span data-stu-id="6e48d-102">CurrencyColumn resource type</span></span>

> <span data-ttu-id="6e48d-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e48d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e48d-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e48d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e48d-105">**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.</span><span class="sxs-lookup"><span data-stu-id="6e48d-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e48d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e48d-106">JSON representation</span></span>

<span data-ttu-id="6e48d-107">Aqui está uma representação JSON de um recurso **currencyColumn**.</span><span class="sxs-lookup"><span data-stu-id="6e48d-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="6e48d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e48d-108">Properties</span></span>

| <span data-ttu-id="6e48d-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6e48d-109">Property name</span></span> | <span data-ttu-id="6e48d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e48d-110">Type</span></span>   | <span data-ttu-id="6e48d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e48d-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="6e48d-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="6e48d-112">**locale**</span></span>    | <span data-ttu-id="6e48d-113">string</span><span class="sxs-lookup"><span data-stu-id="6e48d-113">string</span></span> | <span data-ttu-id="6e48d-114">Especifica a localidade da qual o símbolo de moeda deverá ser inferido.</span><span class="sxs-lookup"><span data-stu-id="6e48d-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
