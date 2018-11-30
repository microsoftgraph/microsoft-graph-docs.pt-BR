---
title: tipo de enum safeSearchFilterType
description: Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
ms.openlocfilehash: cf4f61e1b9e4e9f4fcfd94e6372ce517f3b735e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005230"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="dd124-103">tipo de enum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="dd124-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="dd124-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dd124-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd124-105">Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária</span><span class="sxs-lookup"><span data-stu-id="dd124-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="dd124-106">Membros</span><span class="sxs-lookup"><span data-stu-id="dd124-106">Members</span></span>
|<span data-ttu-id="dd124-107">Membro</span><span class="sxs-lookup"><span data-stu-id="dd124-107">Member</span></span>|<span data-ttu-id="dd124-108">Valor</span><span class="sxs-lookup"><span data-stu-id="dd124-108">Value</span></span>|<span data-ttu-id="dd124-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd124-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd124-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="dd124-110">userDefined</span></span>|<span data-ttu-id="dd124-111">0</span><span class="sxs-lookup"><span data-stu-id="dd124-111">0</span></span>|<span data-ttu-id="dd124-112">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="dd124-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="dd124-113">estrito</span><span class="sxs-lookup"><span data-stu-id="dd124-113">strict</span></span>|<span data-ttu-id="dd124-114">1</span><span class="sxs-lookup"><span data-stu-id="dd124-114">1</span></span>|<span data-ttu-id="dd124-115">Restrito, mais alto de filtragem em relação a conteúdo para adultos.</span><span class="sxs-lookup"><span data-stu-id="dd124-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="dd124-116">moderar</span><span class="sxs-lookup"><span data-stu-id="dd124-116">moderate</span></span>|<span data-ttu-id="dd124-117">2</span><span class="sxs-lookup"><span data-stu-id="dd124-117">2</span></span>|<span data-ttu-id="dd124-118">Moderar filtragem contra conteúdo para adultos (resultados de pesquisa válido não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="dd124-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



