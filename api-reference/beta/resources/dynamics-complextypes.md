---
title: JSON de tipos complexos
description: Tipos de dados complexos no JSON para Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 77d2f7c5c491bf6e86a6df1a05b4a1cdd7788187
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040056"
---
# <a name="complex-types-json"></a><span data-ttu-id="4f941-103">JSON de tipos complexos</span><span class="sxs-lookup"><span data-stu-id="4f941-103">complex types JSON</span></span>

<span data-ttu-id="4f941-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f941-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f941-105">Estes são os vários tipos complexos no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="4f941-105">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="4f941-106">Você pode ver o uso desses tipos complexos nos vários métodos individuais que fazem uso deles.</span><span class="sxs-lookup"><span data-stu-id="4f941-106">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="4f941-107">Endereço postal</span><span class="sxs-lookup"><span data-stu-id="4f941-107">Postal address</span></span>

<span data-ttu-id="4f941-108">Representa um tipo complexo de endereço postal no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="4f941-108">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="4f941-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f941-109">Properties</span></span>
| <span data-ttu-id="4f941-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f941-110">Property</span></span>     | <span data-ttu-id="4f941-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f941-111">Type</span></span>       |<span data-ttu-id="4f941-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f941-112">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="4f941-113">street</span><span class="sxs-lookup"><span data-stu-id="4f941-113">street</span></span>        |<span data-ttu-id="4f941-114">string</span><span class="sxs-lookup"><span data-stu-id="4f941-114">string</span></span>    |<span data-ttu-id="4f941-115">Rua do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="4f941-115">Postal address street.</span></span>  |
|<span data-ttu-id="4f941-116">city</span><span class="sxs-lookup"><span data-stu-id="4f941-116">city</span></span>          |<span data-ttu-id="4f941-117">string</span><span class="sxs-lookup"><span data-stu-id="4f941-117">string</span></span>    |<span data-ttu-id="4f941-118">Cidade do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="4f941-118">Postal address city.</span></span>    |
|<span data-ttu-id="4f941-119">estado</span><span class="sxs-lookup"><span data-stu-id="4f941-119">state</span></span>         |<span data-ttu-id="4f941-120">string</span><span class="sxs-lookup"><span data-stu-id="4f941-120">string</span></span>    |<span data-ttu-id="4f941-121">Estado do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="4f941-121">Postal address state.</span></span>   |
|<span data-ttu-id="4f941-122">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="4f941-122">countryLetterCode</span></span>|<span data-ttu-id="4f941-123">string</span><span class="sxs-lookup"><span data-stu-id="4f941-123">string</span></span> |<span data-ttu-id="4f941-124">Código postal carta de país (palavra de dois caracteres)</span><span class="sxs-lookup"><span data-stu-id="4f941-124">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="4f941-125">postalCode</span><span class="sxs-lookup"><span data-stu-id="4f941-125">postalCode</span></span>    |<span data-ttu-id="4f941-126">string</span><span class="sxs-lookup"><span data-stu-id="4f941-126">string</span></span>    |<span data-ttu-id="4f941-127">Código de post de endereço postal</span><span class="sxs-lookup"><span data-stu-id="4f941-127">Postal address post code</span></span>|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```



