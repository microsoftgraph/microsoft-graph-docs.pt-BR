---
title: tipo de enum safeSearchFilterType
description: Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
author: tfitzmac
ms.openlocfilehash: eb0c7cfb862364ddc4703c89d19ea844ada6466d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343194"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="db95f-103">tipo de enum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="db95f-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="db95f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="db95f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db95f-105">Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária</span><span class="sxs-lookup"><span data-stu-id="db95f-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="db95f-106">Membros</span><span class="sxs-lookup"><span data-stu-id="db95f-106">Members</span></span>
|<span data-ttu-id="db95f-107">Membro</span><span class="sxs-lookup"><span data-stu-id="db95f-107">Member</span></span>|<span data-ttu-id="db95f-108">Valor</span><span class="sxs-lookup"><span data-stu-id="db95f-108">Value</span></span>|<span data-ttu-id="db95f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="db95f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db95f-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="db95f-110">userDefined</span></span>|<span data-ttu-id="db95f-111">0</span><span class="sxs-lookup"><span data-stu-id="db95f-111">0</span></span>|<span data-ttu-id="db95f-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="db95f-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="db95f-113">estrito</span><span class="sxs-lookup"><span data-stu-id="db95f-113">strict</span></span>|<span data-ttu-id="db95f-114">1</span><span class="sxs-lookup"><span data-stu-id="db95f-114">1</span></span>|<span data-ttu-id="db95f-115">Restrito, mais alto de filtragem em relação a conteúdo para adultos.</span><span class="sxs-lookup"><span data-stu-id="db95f-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="db95f-116">moderar</span><span class="sxs-lookup"><span data-stu-id="db95f-116">moderate</span></span>|<span data-ttu-id="db95f-117">2</span><span class="sxs-lookup"><span data-stu-id="db95f-117">2</span></span>|<span data-ttu-id="db95f-118">Moderar filtragem contra conteúdo para adultos (resultados de pesquisa válido não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="db95f-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



