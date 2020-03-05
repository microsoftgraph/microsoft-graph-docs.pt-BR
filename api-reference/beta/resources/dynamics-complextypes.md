---
title: JSON de tipos complexos
description: Tipos de dados complexos no JSON para Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 59aa494c8396d1370dc588b459c7b76f1614e9cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504983"
---
# <a name="complex-types-json"></a><span data-ttu-id="f8c4b-103">JSON de tipos complexos</span><span class="sxs-lookup"><span data-stu-id="f8c4b-103">complex types JSON</span></span>

<span data-ttu-id="f8c4b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f8c4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8c4b-105">Estes são os vários tipos complexos no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="f8c4b-105">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="f8c4b-106">Você pode ver o uso desses tipos complexos nos vários métodos individuais que fazem uso deles.</span><span class="sxs-lookup"><span data-stu-id="f8c4b-106">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="f8c4b-107">Endereço postal</span><span class="sxs-lookup"><span data-stu-id="f8c4b-107">Postal address</span></span>

<span data-ttu-id="f8c4b-108">Representa um tipo complexo de endereço postal no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="f8c4b-108">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="f8c4b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8c4b-109">Properties</span></span>
| <span data-ttu-id="f8c4b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8c4b-110">Property</span></span>     | <span data-ttu-id="f8c4b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8c4b-111">Type</span></span>       |<span data-ttu-id="f8c4b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8c4b-112">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="f8c4b-113">street</span><span class="sxs-lookup"><span data-stu-id="f8c4b-113">street</span></span>        |<span data-ttu-id="f8c4b-114">string</span><span class="sxs-lookup"><span data-stu-id="f8c4b-114">string</span></span>    |<span data-ttu-id="f8c4b-115">Rua do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="f8c4b-115">Postal address street.</span></span>  |
|<span data-ttu-id="f8c4b-116">city</span><span class="sxs-lookup"><span data-stu-id="f8c4b-116">city</span></span>          |<span data-ttu-id="f8c4b-117">string</span><span class="sxs-lookup"><span data-stu-id="f8c4b-117">string</span></span>    |<span data-ttu-id="f8c4b-118">Cidade do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="f8c4b-118">Postal address city.</span></span>    |
|<span data-ttu-id="f8c4b-119">estado</span><span class="sxs-lookup"><span data-stu-id="f8c4b-119">state</span></span>         |<span data-ttu-id="f8c4b-120">string</span><span class="sxs-lookup"><span data-stu-id="f8c4b-120">string</span></span>    |<span data-ttu-id="f8c4b-121">Estado do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="f8c4b-121">Postal address state.</span></span>   |
|<span data-ttu-id="f8c4b-122">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="f8c4b-122">countryLetterCode</span></span>|<span data-ttu-id="f8c4b-123">string</span><span class="sxs-lookup"><span data-stu-id="f8c4b-123">string</span></span> |<span data-ttu-id="f8c4b-124">Código postal carta de país (palavra de dois caracteres)</span><span class="sxs-lookup"><span data-stu-id="f8c4b-124">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="f8c4b-125">postalCode</span><span class="sxs-lookup"><span data-stu-id="f8c4b-125">postalCode</span></span>    |<span data-ttu-id="f8c4b-126">string</span><span class="sxs-lookup"><span data-stu-id="f8c4b-126">string</span></span>    |<span data-ttu-id="f8c4b-127">Código de post de endereço postal</span><span class="sxs-lookup"><span data-stu-id="f8c4b-127">Postal address post code</span></span>|

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

