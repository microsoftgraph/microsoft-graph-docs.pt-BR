---
title: Tipo denum safeSearchFilterType
description: Especifica que nível de pesquisa segura (filtragem de conteúdo adulto) é necessário
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 60463edb06c961e7911b5391ea8b3e4e8f1150ec
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754696"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="ed4a5-103">Tipo denum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="ed4a5-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="ed4a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed4a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed4a5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed4a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed4a5-106">Especifica que nível de pesquisa segura (filtragem de conteúdo adulto) é necessário</span><span class="sxs-lookup"><span data-stu-id="ed4a5-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="ed4a5-107">Membros</span><span class="sxs-lookup"><span data-stu-id="ed4a5-107">Members</span></span>
|<span data-ttu-id="ed4a5-108">Membro</span><span class="sxs-lookup"><span data-stu-id="ed4a5-108">Member</span></span>|<span data-ttu-id="ed4a5-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ed4a5-109">Value</span></span>|<span data-ttu-id="ed4a5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed4a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed4a5-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="ed4a5-111">userDefined</span></span>|<span data-ttu-id="ed4a5-112">0</span><span class="sxs-lookup"><span data-stu-id="ed4a5-112">0</span></span>|<span data-ttu-id="ed4a5-113">User Defined, default value, no intent.</span><span class="sxs-lookup"><span data-stu-id="ed4a5-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ed4a5-114">strict</span><span class="sxs-lookup"><span data-stu-id="ed4a5-114">strict</span></span>|<span data-ttu-id="ed4a5-115">1</span><span class="sxs-lookup"><span data-stu-id="ed4a5-115">1</span></span>|<span data-ttu-id="ed4a5-116">Filtragem estrita e mais alta em relação ao conteúdo adulto.</span><span class="sxs-lookup"><span data-stu-id="ed4a5-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="ed4a5-117">moderada</span><span class="sxs-lookup"><span data-stu-id="ed4a5-117">moderate</span></span>|<span data-ttu-id="ed4a5-118">2</span><span class="sxs-lookup"><span data-stu-id="ed4a5-118">2</span></span>|<span data-ttu-id="ed4a5-119">Filtragem moderada em relação ao conteúdo adulto (os resultados válidos da pesquisa não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="ed4a5-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




