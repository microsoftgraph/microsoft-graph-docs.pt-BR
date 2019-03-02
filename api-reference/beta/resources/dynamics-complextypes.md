---
title: JSON de tipos complexos
description: Tipos de dados complexos no JSON para Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366764"
---
# <a name="complex-types-json"></a><span data-ttu-id="466e9-103">JSON de tipos complexos</span><span class="sxs-lookup"><span data-stu-id="466e9-103">complex types JSON</span></span>
<span data-ttu-id="466e9-104">Estes são os vários tipos complexos no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="466e9-104">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="466e9-105">Você pode ver o uso desses tipos complexos nos vários métodos individuais que fazem uso deles.</span><span class="sxs-lookup"><span data-stu-id="466e9-105">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="466e9-106">Endereço postal</span><span class="sxs-lookup"><span data-stu-id="466e9-106">Postal address</span></span>

<span data-ttu-id="466e9-107">Representa um tipo complexo de endereço postal no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="466e9-107">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="466e9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="466e9-108">Properties</span></span>
| <span data-ttu-id="466e9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="466e9-109">Property</span></span>     | <span data-ttu-id="466e9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="466e9-110">Type</span></span>       |<span data-ttu-id="466e9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="466e9-111">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="466e9-112">street</span><span class="sxs-lookup"><span data-stu-id="466e9-112">street</span></span>        |<span data-ttu-id="466e9-113">string</span><span class="sxs-lookup"><span data-stu-id="466e9-113">string</span></span>    |<span data-ttu-id="466e9-114">Rua do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="466e9-114">Postal address street.</span></span>  |
|<span data-ttu-id="466e9-115">city</span><span class="sxs-lookup"><span data-stu-id="466e9-115">city</span></span>          |<span data-ttu-id="466e9-116">string</span><span class="sxs-lookup"><span data-stu-id="466e9-116">string</span></span>    |<span data-ttu-id="466e9-117">Cidade do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="466e9-117">Postal address city.</span></span>    |
|<span data-ttu-id="466e9-118">state</span><span class="sxs-lookup"><span data-stu-id="466e9-118">state</span></span>         |<span data-ttu-id="466e9-119">string</span><span class="sxs-lookup"><span data-stu-id="466e9-119">string</span></span>    |<span data-ttu-id="466e9-120">Estado do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="466e9-120">Postal address state.</span></span>   |
|<span data-ttu-id="466e9-121">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="466e9-121">countryLetterCode</span></span>|<span data-ttu-id="466e9-122">string</span><span class="sxs-lookup"><span data-stu-id="466e9-122">string</span></span> |<span data-ttu-id="466e9-123">Código postal carta de país (palavra de dois caracteres)</span><span class="sxs-lookup"><span data-stu-id="466e9-123">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="466e9-124">postalCode</span><span class="sxs-lookup"><span data-stu-id="466e9-124">postalCode</span></span>    |<span data-ttu-id="466e9-125">string</span><span class="sxs-lookup"><span data-stu-id="466e9-125">string</span></span>    |<span data-ttu-id="466e9-126">Código de post de endereço postal</span><span class="sxs-lookup"><span data-stu-id="466e9-126">Postal address post code</span></span>|

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

