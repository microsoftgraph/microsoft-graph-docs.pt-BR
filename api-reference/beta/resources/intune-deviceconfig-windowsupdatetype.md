---
title: tipo de enum windowsUpdateType
description: Quais dispositivos de filial receberão suas atualizações do
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1444af64043ac38685ca022b56b8856be77a0b70
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944345"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="42994-103">tipo de enum windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="42994-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="42994-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="42994-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42994-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="42994-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42994-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="42994-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42994-107">Quais dispositivos de filial receberão suas atualizações do</span><span class="sxs-lookup"><span data-stu-id="42994-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="42994-108">Membros</span><span class="sxs-lookup"><span data-stu-id="42994-108">Members</span></span>
|<span data-ttu-id="42994-109">Membro</span><span class="sxs-lookup"><span data-stu-id="42994-109">Member</span></span>|<span data-ttu-id="42994-110">Valor</span><span class="sxs-lookup"><span data-stu-id="42994-110">Value</span></span>|<span data-ttu-id="42994-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42994-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42994-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="42994-112">userDefined</span></span>|<span data-ttu-id="42994-113">0</span><span class="sxs-lookup"><span data-stu-id="42994-113">0</span></span>|<span data-ttu-id="42994-114">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="42994-114">Allow the user to set.</span></span>|
|<span data-ttu-id="42994-115">todos os</span><span class="sxs-lookup"><span data-stu-id="42994-115">all</span></span>|<span data-ttu-id="42994-116">1</span><span class="sxs-lookup"><span data-stu-id="42994-116">1</span></span>|<span data-ttu-id="42994-117">O canal delimitadas anual (público alvo).</span><span class="sxs-lookup"><span data-stu-id="42994-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="42994-118">Dispositivo obtém todas as atualizações aplicáveis de recurso do canal delimitadas anual (multidifusão).</span><span class="sxs-lookup"><span data-stu-id="42994-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="42994-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="42994-119">businessReadyOnly</span></span>|<span data-ttu-id="42994-120">2</span><span class="sxs-lookup"><span data-stu-id="42994-120">2</span></span>|<span data-ttu-id="42994-121">Canal delimitadas anual.</span><span class="sxs-lookup"><span data-stu-id="42994-121">Semi-annual Channel.</span></span> <span data-ttu-id="42994-122">Dispositivo obtém atualizações de recurso do canal delimitadas anual.</span><span class="sxs-lookup"><span data-stu-id="42994-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="42994-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="42994-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="42994-124">3</span><span class="sxs-lookup"><span data-stu-id="42994-124">3</span></span>|<span data-ttu-id="42994-125">Construir Insider Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="42994-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="42994-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="42994-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="42994-127">4</span><span class="sxs-lookup"><span data-stu-id="42994-127">4</span></span>|<span data-ttu-id="42994-128">Construir Insider Windows - lento</span><span class="sxs-lookup"><span data-stu-id="42994-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="42994-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="42994-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="42994-130">5</span><span class="sxs-lookup"><span data-stu-id="42994-130">5</span></span>|<span data-ttu-id="42994-131">Criação de Insider Windows versão</span><span class="sxs-lookup"><span data-stu-id="42994-131">Release Windows Insider build</span></span>|





