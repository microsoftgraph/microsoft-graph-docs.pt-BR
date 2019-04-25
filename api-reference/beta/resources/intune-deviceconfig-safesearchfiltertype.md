---
title: tipo de enumeração safeSearchFilterType
description: Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 564e641fcdc7e0d06d48666881fc3bcedfe3505c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573211"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="c02ac-103">tipo de enumeração safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="c02ac-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="c02ac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c02ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c02ac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c02ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c02ac-106">Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário</span><span class="sxs-lookup"><span data-stu-id="c02ac-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="c02ac-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c02ac-107">Members</span></span>
|<span data-ttu-id="c02ac-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c02ac-108">Member</span></span>|<span data-ttu-id="c02ac-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c02ac-109">Value</span></span>|<span data-ttu-id="c02ac-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c02ac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c02ac-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="c02ac-111">userDefined</span></span>|<span data-ttu-id="c02ac-112">,0</span><span class="sxs-lookup"><span data-stu-id="c02ac-112">0</span></span>|<span data-ttu-id="c02ac-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c02ac-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c02ac-114">impede</span><span class="sxs-lookup"><span data-stu-id="c02ac-114">strict</span></span>|<span data-ttu-id="c02ac-115">1 </span><span class="sxs-lookup"><span data-stu-id="c02ac-115">1</span></span>|<span data-ttu-id="c02ac-116">Filtragem mais rigorosa e estrita contra conteúdo adulto.</span><span class="sxs-lookup"><span data-stu-id="c02ac-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="c02ac-117">moderado</span><span class="sxs-lookup"><span data-stu-id="c02ac-117">moderate</span></span>|<span data-ttu-id="c02ac-118">2 </span><span class="sxs-lookup"><span data-stu-id="c02ac-118">2</span></span>|<span data-ttu-id="c02ac-119">Filtragem moderada contra conteúdo adulto (os resultados de pesquisa válidos não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="c02ac-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





