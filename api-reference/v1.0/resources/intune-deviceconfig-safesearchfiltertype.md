---
title: tipo de enumeração safeSearchFilterType
description: Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c82f80f6081f57a88fcdf26f7639277d72b5e0d8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250583"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="02a10-103">tipo de enumeração safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="02a10-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="02a10-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02a10-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02a10-105">Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário</span><span class="sxs-lookup"><span data-stu-id="02a10-105">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="02a10-106">Membros</span><span class="sxs-lookup"><span data-stu-id="02a10-106">Members</span></span>
|<span data-ttu-id="02a10-107">Membro</span><span class="sxs-lookup"><span data-stu-id="02a10-107">Member</span></span>|<span data-ttu-id="02a10-108">Valor</span><span class="sxs-lookup"><span data-stu-id="02a10-108">Value</span></span>|<span data-ttu-id="02a10-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="02a10-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a10-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="02a10-110">userDefined</span></span>|<span data-ttu-id="02a10-111">,0</span><span class="sxs-lookup"><span data-stu-id="02a10-111">0</span></span>|<span data-ttu-id="02a10-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="02a10-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="02a10-113">impede</span><span class="sxs-lookup"><span data-stu-id="02a10-113">strict</span></span>|<span data-ttu-id="02a10-114">1</span><span class="sxs-lookup"><span data-stu-id="02a10-114">1</span></span>|<span data-ttu-id="02a10-115">Filtragem mais rigorosa e estrita contra conteúdo adulto.</span><span class="sxs-lookup"><span data-stu-id="02a10-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="02a10-116">moderado</span><span class="sxs-lookup"><span data-stu-id="02a10-116">moderate</span></span>|<span data-ttu-id="02a10-117">duas</span><span class="sxs-lookup"><span data-stu-id="02a10-117">2</span></span>|<span data-ttu-id="02a10-118">Filtragem moderada contra conteúdo adulto (os resultados de pesquisa válidos não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="02a10-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



