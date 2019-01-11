---
title: tipo de enum safeSearchFilterType
description: Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28aea918c35bb9d90f514e4a8838f219c212405b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830853"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="a6679-103">tipo de enum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="a6679-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="a6679-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a6679-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6679-105">Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária</span><span class="sxs-lookup"><span data-stu-id="a6679-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="a6679-106">Membros</span><span class="sxs-lookup"><span data-stu-id="a6679-106">Members</span></span>
|<span data-ttu-id="a6679-107">Membro</span><span class="sxs-lookup"><span data-stu-id="a6679-107">Member</span></span>|<span data-ttu-id="a6679-108">Valor</span><span class="sxs-lookup"><span data-stu-id="a6679-108">Value</span></span>|<span data-ttu-id="a6679-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6679-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6679-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="a6679-110">userDefined</span></span>|<span data-ttu-id="a6679-111">0</span><span class="sxs-lookup"><span data-stu-id="a6679-111">0</span></span>|<span data-ttu-id="a6679-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="a6679-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a6679-113">estrito</span><span class="sxs-lookup"><span data-stu-id="a6679-113">strict</span></span>|<span data-ttu-id="a6679-114">1</span><span class="sxs-lookup"><span data-stu-id="a6679-114">1</span></span>|<span data-ttu-id="a6679-115">Restrito, mais alto de filtragem em relação a conteúdo para adultos.</span><span class="sxs-lookup"><span data-stu-id="a6679-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="a6679-116">moderar</span><span class="sxs-lookup"><span data-stu-id="a6679-116">moderate</span></span>|<span data-ttu-id="a6679-117">2</span><span class="sxs-lookup"><span data-stu-id="a6679-117">2</span></span>|<span data-ttu-id="a6679-118">Moderar filtragem contra conteúdo para adultos (resultados de pesquisa válido não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="a6679-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



