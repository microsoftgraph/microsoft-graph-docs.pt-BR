---
title: tipo de enumeração safeSearchFilterType
description: Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 54beae59c3341605b8b4a7c3f482c8d98d31851b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293896"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="120e8-103">tipo de enumeração safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="120e8-103">safeSearchFilterType enum type</span></span>

<span data-ttu-id="120e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="120e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="120e8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="120e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="120e8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="120e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="120e8-107">Especifica o nível de pesquisa segura (filtragem de conteúdo adulto) é necessário</span><span class="sxs-lookup"><span data-stu-id="120e8-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="120e8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="120e8-108">Members</span></span>
|<span data-ttu-id="120e8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="120e8-109">Member</span></span>|<span data-ttu-id="120e8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="120e8-110">Value</span></span>|<span data-ttu-id="120e8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="120e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="120e8-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="120e8-112">userDefined</span></span>|<span data-ttu-id="120e8-113">,0</span><span class="sxs-lookup"><span data-stu-id="120e8-113">0</span></span>|<span data-ttu-id="120e8-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="120e8-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="120e8-115">impede</span><span class="sxs-lookup"><span data-stu-id="120e8-115">strict</span></span>|<span data-ttu-id="120e8-116">1</span><span class="sxs-lookup"><span data-stu-id="120e8-116">1</span></span>|<span data-ttu-id="120e8-117">Filtragem mais rigorosa e estrita contra conteúdo adulto.</span><span class="sxs-lookup"><span data-stu-id="120e8-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="120e8-118">moderado</span><span class="sxs-lookup"><span data-stu-id="120e8-118">moderate</span></span>|<span data-ttu-id="120e8-119">duas</span><span class="sxs-lookup"><span data-stu-id="120e8-119">2</span></span>|<span data-ttu-id="120e8-120">Filtragem moderada contra conteúdo adulto (os resultados de pesquisa válidos não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="120e8-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




