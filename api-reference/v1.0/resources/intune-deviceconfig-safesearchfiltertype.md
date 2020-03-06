---
title: tipo de enumeração safeSearchFilterType
description: Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c8ef86709169448d58bde53507747377526c38ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530469"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="b50dd-103">tipo de enumeração safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="b50dd-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="b50dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b50dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b50dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b50dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b50dd-106">Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário</span><span class="sxs-lookup"><span data-stu-id="b50dd-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="b50dd-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b50dd-107">Members</span></span>
|<span data-ttu-id="b50dd-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b50dd-108">Member</span></span>|<span data-ttu-id="b50dd-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b50dd-109">Value</span></span>|<span data-ttu-id="b50dd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b50dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b50dd-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="b50dd-111">userDefined</span></span>|<span data-ttu-id="b50dd-112">,0</span><span class="sxs-lookup"><span data-stu-id="b50dd-112">0</span></span>|<span data-ttu-id="b50dd-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="b50dd-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b50dd-114">impede</span><span class="sxs-lookup"><span data-stu-id="b50dd-114">strict</span></span>|<span data-ttu-id="b50dd-115">1 </span><span class="sxs-lookup"><span data-stu-id="b50dd-115">1</span></span>|<span data-ttu-id="b50dd-116">Filtragem mais rigorosa e estrita contra conteúdo adulto.</span><span class="sxs-lookup"><span data-stu-id="b50dd-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="b50dd-117">moderado</span><span class="sxs-lookup"><span data-stu-id="b50dd-117">moderate</span></span>|<span data-ttu-id="b50dd-118">2 </span><span class="sxs-lookup"><span data-stu-id="b50dd-118">2</span></span>|<span data-ttu-id="b50dd-119">Filtragem moderada contra conteúdo adulto (os resultados de pesquisa válidos não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="b50dd-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




