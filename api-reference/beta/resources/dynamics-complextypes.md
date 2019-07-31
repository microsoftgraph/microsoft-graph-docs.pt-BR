---
title: JSON de tipos complexos
description: Tipos de dados complexos no JSON para Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bb61450ab7f1d62d459f525f6341093f25b1686f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012636"
---
# <a name="complex-types-json"></a><span data-ttu-id="3db86-103">JSON de tipos complexos</span><span class="sxs-lookup"><span data-stu-id="3db86-103">complex types JSON</span></span>
<span data-ttu-id="3db86-104">Estes são os vários tipos complexos no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="3db86-104">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="3db86-105">Você pode ver o uso desses tipos complexos nos vários métodos individuais que fazem uso deles.</span><span class="sxs-lookup"><span data-stu-id="3db86-105">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="3db86-106">Endereço postal</span><span class="sxs-lookup"><span data-stu-id="3db86-106">Postal address</span></span>

<span data-ttu-id="3db86-107">Representa um tipo complexo de endereço postal no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="3db86-107">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="3db86-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3db86-108">Properties</span></span>
| <span data-ttu-id="3db86-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3db86-109">Property</span></span>     | <span data-ttu-id="3db86-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3db86-110">Type</span></span>       |<span data-ttu-id="3db86-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3db86-111">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="3db86-112">street</span><span class="sxs-lookup"><span data-stu-id="3db86-112">street</span></span>        |<span data-ttu-id="3db86-113">string</span><span class="sxs-lookup"><span data-stu-id="3db86-113">string</span></span>    |<span data-ttu-id="3db86-114">Rua do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="3db86-114">Postal address street.</span></span>  |
|<span data-ttu-id="3db86-115">city</span><span class="sxs-lookup"><span data-stu-id="3db86-115">city</span></span>          |<span data-ttu-id="3db86-116">string</span><span class="sxs-lookup"><span data-stu-id="3db86-116">string</span></span>    |<span data-ttu-id="3db86-117">Cidade do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="3db86-117">Postal address city.</span></span>    |
|<span data-ttu-id="3db86-118">estado</span><span class="sxs-lookup"><span data-stu-id="3db86-118">state</span></span>         |<span data-ttu-id="3db86-119">string</span><span class="sxs-lookup"><span data-stu-id="3db86-119">string</span></span>    |<span data-ttu-id="3db86-120">Estado do endereço postal.</span><span class="sxs-lookup"><span data-stu-id="3db86-120">Postal address state.</span></span>   |
|<span data-ttu-id="3db86-121">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="3db86-121">countryLetterCode</span></span>|<span data-ttu-id="3db86-122">string</span><span class="sxs-lookup"><span data-stu-id="3db86-122">string</span></span> |<span data-ttu-id="3db86-123">Código postal carta de país (palavra de dois caracteres)</span><span class="sxs-lookup"><span data-stu-id="3db86-123">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="3db86-124">postalCode</span><span class="sxs-lookup"><span data-stu-id="3db86-124">postalCode</span></span>    |<span data-ttu-id="3db86-125">string</span><span class="sxs-lookup"><span data-stu-id="3db86-125">string</span></span>    |<span data-ttu-id="3db86-126">Código de post de endereço postal</span><span class="sxs-lookup"><span data-stu-id="3db86-126">Postal address post code</span></span>|

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

