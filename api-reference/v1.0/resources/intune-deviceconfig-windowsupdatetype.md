---
title: tipo de enum windowsUpdateType
description: Quais dispositivos de filial receberão suas atualizações do
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90d1f946dd497e650df5eb07004560dda028e14f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930338"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="23219-103">tipo de enum windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="23219-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="23219-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="23219-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23219-105">Quais dispositivos de filial receberão suas atualizações do</span><span class="sxs-lookup"><span data-stu-id="23219-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="23219-106">Membros</span><span class="sxs-lookup"><span data-stu-id="23219-106">Members</span></span>
|<span data-ttu-id="23219-107">Membro</span><span class="sxs-lookup"><span data-stu-id="23219-107">Member</span></span>|<span data-ttu-id="23219-108">Valor</span><span class="sxs-lookup"><span data-stu-id="23219-108">Value</span></span>|<span data-ttu-id="23219-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="23219-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23219-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="23219-110">userDefined</span></span>|<span data-ttu-id="23219-111">0</span><span class="sxs-lookup"><span data-stu-id="23219-111">0</span></span>|<span data-ttu-id="23219-112">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="23219-112">Allow the user to set.</span></span>|
|<span data-ttu-id="23219-113">todos os</span><span class="sxs-lookup"><span data-stu-id="23219-113">all</span></span>|<span data-ttu-id="23219-114">1</span><span class="sxs-lookup"><span data-stu-id="23219-114">1</span></span>|<span data-ttu-id="23219-115">O canal delimitadas anual (público alvo).</span><span class="sxs-lookup"><span data-stu-id="23219-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="23219-116">Dispositivo obtém todas as atualizações aplicáveis de recurso do canal delimitadas anual (multidifusão).</span><span class="sxs-lookup"><span data-stu-id="23219-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="23219-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="23219-117">businessReadyOnly</span></span>|<span data-ttu-id="23219-118">2</span><span class="sxs-lookup"><span data-stu-id="23219-118">2</span></span>|<span data-ttu-id="23219-119">Canal delimitadas anual.</span><span class="sxs-lookup"><span data-stu-id="23219-119">Semi-annual Channel.</span></span> <span data-ttu-id="23219-120">Dispositivo obtém atualizações de recurso do canal delimitadas anual.</span><span class="sxs-lookup"><span data-stu-id="23219-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="23219-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="23219-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="23219-122">3</span><span class="sxs-lookup"><span data-stu-id="23219-122">3</span></span>|<span data-ttu-id="23219-123">Construir Insider Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="23219-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="23219-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="23219-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="23219-125">4</span><span class="sxs-lookup"><span data-stu-id="23219-125">4</span></span>|<span data-ttu-id="23219-126">Construir Insider Windows - lento</span><span class="sxs-lookup"><span data-stu-id="23219-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="23219-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="23219-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="23219-128">5</span><span class="sxs-lookup"><span data-stu-id="23219-128">5</span></span>|<span data-ttu-id="23219-129">Criação de Insider Windows versão</span><span class="sxs-lookup"><span data-stu-id="23219-129">Release Windows Insider build</span></span>|



