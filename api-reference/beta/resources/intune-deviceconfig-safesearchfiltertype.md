---
title: tipo de enumeração safeSearchFilterType
description: Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8585745d2f4e9c529e6ef56c9ce209b1da67f2ac
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444874"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="c376a-103">tipo de enumeração safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="c376a-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="c376a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c376a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c376a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c376a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c376a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c376a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c376a-107">Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário</span><span class="sxs-lookup"><span data-stu-id="c376a-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="c376a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c376a-108">Members</span></span>
|<span data-ttu-id="c376a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c376a-109">Member</span></span>|<span data-ttu-id="c376a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c376a-110">Value</span></span>|<span data-ttu-id="c376a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c376a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c376a-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="c376a-112">userDefined</span></span>|<span data-ttu-id="c376a-113">,0</span><span class="sxs-lookup"><span data-stu-id="c376a-113">0</span></span>|<span data-ttu-id="c376a-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c376a-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c376a-115">impede</span><span class="sxs-lookup"><span data-stu-id="c376a-115">strict</span></span>|<span data-ttu-id="c376a-116">1</span><span class="sxs-lookup"><span data-stu-id="c376a-116">1</span></span>|<span data-ttu-id="c376a-117">Filtragem mais rigorosa e estrita contra conteúdo adulto.</span><span class="sxs-lookup"><span data-stu-id="c376a-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="c376a-118">moderado</span><span class="sxs-lookup"><span data-stu-id="c376a-118">moderate</span></span>|<span data-ttu-id="c376a-119">duas</span><span class="sxs-lookup"><span data-stu-id="c376a-119">2</span></span>|<span data-ttu-id="c376a-120">Filtragem moderada contra conteúdo adulto (os resultados de pesquisa válidos não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="c376a-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



