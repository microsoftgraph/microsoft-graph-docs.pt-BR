---
title: tipo de enum windowsUpdateType
description: Quais dispositivos de filial receberão suas atualizações do
author: tfitzmac
ms.openlocfilehash: b41fea0254cbbb6a590d240c2db9e4fb7aa0e6eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309622"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="d629e-103">tipo de enum windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="d629e-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="d629e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d629e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d629e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d629e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d629e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d629e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d629e-107">Quais dispositivos de filial receberão suas atualizações do</span><span class="sxs-lookup"><span data-stu-id="d629e-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="d629e-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d629e-108">Members</span></span>
|<span data-ttu-id="d629e-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d629e-109">Member</span></span>|<span data-ttu-id="d629e-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d629e-110">Value</span></span>|<span data-ttu-id="d629e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d629e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d629e-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="d629e-112">userDefined</span></span>|<span data-ttu-id="d629e-113">0</span><span class="sxs-lookup"><span data-stu-id="d629e-113">0</span></span>|<span data-ttu-id="d629e-114">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="d629e-114">Allow the user to set.</span></span>|
|<span data-ttu-id="d629e-115">todos os</span><span class="sxs-lookup"><span data-stu-id="d629e-115">all</span></span>|<span data-ttu-id="d629e-116">1</span><span class="sxs-lookup"><span data-stu-id="d629e-116">1</span></span>|<span data-ttu-id="d629e-117">O canal delimitadas anual (público alvo).</span><span class="sxs-lookup"><span data-stu-id="d629e-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="d629e-118">Dispositivo obtém todas as atualizações aplicáveis de recurso do canal delimitadas anual (multidifusão).</span><span class="sxs-lookup"><span data-stu-id="d629e-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="d629e-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="d629e-119">businessReadyOnly</span></span>|<span data-ttu-id="d629e-120">2</span><span class="sxs-lookup"><span data-stu-id="d629e-120">2</span></span>|<span data-ttu-id="d629e-121">Canal delimitadas anual.</span><span class="sxs-lookup"><span data-stu-id="d629e-121">Semi-annual Channel.</span></span> <span data-ttu-id="d629e-122">Dispositivo obtém atualizações de recurso do canal delimitadas anual.</span><span class="sxs-lookup"><span data-stu-id="d629e-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="d629e-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="d629e-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="d629e-124">3</span><span class="sxs-lookup"><span data-stu-id="d629e-124">3</span></span>|<span data-ttu-id="d629e-125">Construir Insider Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="d629e-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="d629e-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="d629e-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="d629e-127">4</span><span class="sxs-lookup"><span data-stu-id="d629e-127">4</span></span>|<span data-ttu-id="d629e-128">Construir Insider Windows - lento</span><span class="sxs-lookup"><span data-stu-id="d629e-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="d629e-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="d629e-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="d629e-130">5</span><span class="sxs-lookup"><span data-stu-id="d629e-130">5</span></span>|<span data-ttu-id="d629e-131">Criação de Insider Windows versão</span><span class="sxs-lookup"><span data-stu-id="d629e-131">Release Windows Insider build</span></span>|





