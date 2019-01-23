---
title: tipo de enum windowsUpdateType
description: Quais dispositivos de filial receberão suas atualizações do
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d3dd0f6d8ba46d7f1cc803b217a98a862602149
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400134"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="2c0a6-103">tipo de enum windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="2c0a6-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="2c0a6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2c0a6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2c0a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2c0a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c0a6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2c0a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c0a6-107">Quais dispositivos de filial receberão suas atualizações do</span><span class="sxs-lookup"><span data-stu-id="2c0a6-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="2c0a6-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2c0a6-108">Members</span></span>
|<span data-ttu-id="2c0a6-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2c0a6-109">Member</span></span>|<span data-ttu-id="2c0a6-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2c0a6-110">Value</span></span>|<span data-ttu-id="2c0a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c0a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c0a6-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="2c0a6-112">userDefined</span></span>|<span data-ttu-id="2c0a6-113">0</span><span class="sxs-lookup"><span data-stu-id="2c0a6-113">0</span></span>|<span data-ttu-id="2c0a6-114">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="2c0a6-114">Allow the user to set.</span></span>|
|<span data-ttu-id="2c0a6-115">todos os</span><span class="sxs-lookup"><span data-stu-id="2c0a6-115">all</span></span>|<span data-ttu-id="2c0a6-116">1</span><span class="sxs-lookup"><span data-stu-id="2c0a6-116">1</span></span>|<span data-ttu-id="2c0a6-117">O canal delimitadas anual (público alvo).</span><span class="sxs-lookup"><span data-stu-id="2c0a6-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="2c0a6-118">Dispositivo obtém todas as atualizações aplicáveis de recurso do canal delimitadas anual (multidifusão).</span><span class="sxs-lookup"><span data-stu-id="2c0a6-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="2c0a6-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="2c0a6-119">businessReadyOnly</span></span>|<span data-ttu-id="2c0a6-120">2</span><span class="sxs-lookup"><span data-stu-id="2c0a6-120">2</span></span>|<span data-ttu-id="2c0a6-121">Canal delimitadas anual.</span><span class="sxs-lookup"><span data-stu-id="2c0a6-121">Semi-annual Channel.</span></span> <span data-ttu-id="2c0a6-122">Dispositivo obtém atualizações de recurso do canal delimitadas anual.</span><span class="sxs-lookup"><span data-stu-id="2c0a6-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="2c0a6-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="2c0a6-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="2c0a6-124">3</span><span class="sxs-lookup"><span data-stu-id="2c0a6-124">3</span></span>|<span data-ttu-id="2c0a6-125">Construir Insider Windows - Fast</span><span class="sxs-lookup"><span data-stu-id="2c0a6-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="2c0a6-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="2c0a6-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="2c0a6-127">4</span><span class="sxs-lookup"><span data-stu-id="2c0a6-127">4</span></span>|<span data-ttu-id="2c0a6-128">Construir Insider Windows - lento</span><span class="sxs-lookup"><span data-stu-id="2c0a6-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="2c0a6-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="2c0a6-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="2c0a6-130">5</span><span class="sxs-lookup"><span data-stu-id="2c0a6-130">5</span></span>|<span data-ttu-id="2c0a6-131">Criação de Insider Windows versão</span><span class="sxs-lookup"><span data-stu-id="2c0a6-131">Release Windows Insider build</span></span>|




