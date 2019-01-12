---
title: tipo de enum safeSearchFilterType
description: Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 788a266cdd0161ce1cfef426a7fcf4d9726e3324
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964610"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="a7810-103">tipo de enum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="a7810-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="a7810-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a7810-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7810-105">Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária</span><span class="sxs-lookup"><span data-stu-id="a7810-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="a7810-106">Membros</span><span class="sxs-lookup"><span data-stu-id="a7810-106">Members</span></span>
|<span data-ttu-id="a7810-107">Membro</span><span class="sxs-lookup"><span data-stu-id="a7810-107">Member</span></span>|<span data-ttu-id="a7810-108">Valor</span><span class="sxs-lookup"><span data-stu-id="a7810-108">Value</span></span>|<span data-ttu-id="a7810-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7810-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7810-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="a7810-110">userDefined</span></span>|<span data-ttu-id="a7810-111">0</span><span class="sxs-lookup"><span data-stu-id="a7810-111">0</span></span>|<span data-ttu-id="a7810-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="a7810-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a7810-113">estrito</span><span class="sxs-lookup"><span data-stu-id="a7810-113">strict</span></span>|<span data-ttu-id="a7810-114">1</span><span class="sxs-lookup"><span data-stu-id="a7810-114">1</span></span>|<span data-ttu-id="a7810-115">Restrito, mais alto de filtragem em relação a conteúdo para adultos.</span><span class="sxs-lookup"><span data-stu-id="a7810-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="a7810-116">moderar</span><span class="sxs-lookup"><span data-stu-id="a7810-116">moderate</span></span>|<span data-ttu-id="a7810-117">2</span><span class="sxs-lookup"><span data-stu-id="a7810-117">2</span></span>|<span data-ttu-id="a7810-118">Moderar filtragem contra conteúdo para adultos (resultados de pesquisa válido não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="a7810-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



