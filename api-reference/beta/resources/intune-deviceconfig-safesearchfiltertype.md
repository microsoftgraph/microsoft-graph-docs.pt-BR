---
title: tipo de enum safeSearchFilterType
description: Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
ms.openlocfilehash: 71a59574fd98e2571a33e58415acb612f32326a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034394"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="3a731-103">tipo de enum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="3a731-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="3a731-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a731-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a731-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a731-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a731-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3a731-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a731-107">Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária</span><span class="sxs-lookup"><span data-stu-id="3a731-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="3a731-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3a731-108">Members</span></span>
|<span data-ttu-id="3a731-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3a731-109">Member</span></span>|<span data-ttu-id="3a731-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3a731-110">Value</span></span>|<span data-ttu-id="3a731-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a731-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a731-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="3a731-112">userDefined</span></span>|<span data-ttu-id="3a731-113">0</span><span class="sxs-lookup"><span data-stu-id="3a731-113">0</span></span>|<span data-ttu-id="3a731-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="3a731-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="3a731-115">estrito</span><span class="sxs-lookup"><span data-stu-id="3a731-115">strict</span></span>|<span data-ttu-id="3a731-116">1</span><span class="sxs-lookup"><span data-stu-id="3a731-116">1</span></span>|<span data-ttu-id="3a731-117">Restrito, mais alto de filtragem em relação a conteúdo para adultos.</span><span class="sxs-lookup"><span data-stu-id="3a731-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="3a731-118">moderar</span><span class="sxs-lookup"><span data-stu-id="3a731-118">moderate</span></span>|<span data-ttu-id="3a731-119">2</span><span class="sxs-lookup"><span data-stu-id="3a731-119">2</span></span>|<span data-ttu-id="3a731-120">Moderar filtragem contra conteúdo para adultos (resultados de pesquisa válido não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="3a731-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





