---
title: tipo de enum safeSearchFilterType
description: Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária
author: tfitzmac
ms.openlocfilehash: 7bec68919b6af5d773c34caadaf0c1d85b0f5224
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351412"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="70e07-103">tipo de enum safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="70e07-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="70e07-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="70e07-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70e07-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="70e07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70e07-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="70e07-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70e07-107">Especifica qual nível de pesquisa segura (filtragem de conteúdo para adultos) é necessária</span><span class="sxs-lookup"><span data-stu-id="70e07-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="70e07-108">Membros</span><span class="sxs-lookup"><span data-stu-id="70e07-108">Members</span></span>
|<span data-ttu-id="70e07-109">Membro</span><span class="sxs-lookup"><span data-stu-id="70e07-109">Member</span></span>|<span data-ttu-id="70e07-110">Valor</span><span class="sxs-lookup"><span data-stu-id="70e07-110">Value</span></span>|<span data-ttu-id="70e07-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="70e07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70e07-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="70e07-112">userDefined</span></span>|<span data-ttu-id="70e07-113">0</span><span class="sxs-lookup"><span data-stu-id="70e07-113">0</span></span>|<span data-ttu-id="70e07-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="70e07-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="70e07-115">estrito</span><span class="sxs-lookup"><span data-stu-id="70e07-115">strict</span></span>|<span data-ttu-id="70e07-116">1</span><span class="sxs-lookup"><span data-stu-id="70e07-116">1</span></span>|<span data-ttu-id="70e07-117">Restrito, mais alto de filtragem em relação a conteúdo para adultos.</span><span class="sxs-lookup"><span data-stu-id="70e07-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="70e07-118">moderar</span><span class="sxs-lookup"><span data-stu-id="70e07-118">moderate</span></span>|<span data-ttu-id="70e07-119">2</span><span class="sxs-lookup"><span data-stu-id="70e07-119">2</span></span>|<span data-ttu-id="70e07-120">Moderar filtragem contra conteúdo para adultos (resultados de pesquisa válido não serão filtrados).</span><span class="sxs-lookup"><span data-stu-id="70e07-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





