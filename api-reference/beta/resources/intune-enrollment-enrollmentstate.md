---
title: tipo de enum enrollmentState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94a3790733067598442af615cb90b8ae347fd228
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869017"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="3e06e-103">tipo de enum enrollmentState</span><span class="sxs-lookup"><span data-stu-id="3e06e-103">enrollmentState enum type</span></span>

> <span data-ttu-id="3e06e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e06e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e06e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e06e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e06e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3e06e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e06e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e06e-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="3e06e-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3e06e-108">Members</span></span>
|<span data-ttu-id="3e06e-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3e06e-109">Member</span></span>|<span data-ttu-id="3e06e-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3e06e-110">Value</span></span>|<span data-ttu-id="3e06e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e06e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e06e-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3e06e-112">unknown</span></span>|<span data-ttu-id="3e06e-113">0</span><span class="sxs-lookup"><span data-stu-id="3e06e-113">0</span></span>|<span data-ttu-id="3e06e-114">O estado de inscrição do dispositivo é desconhecido</span><span class="sxs-lookup"><span data-stu-id="3e06e-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="3e06e-115">inscritos</span><span class="sxs-lookup"><span data-stu-id="3e06e-115">enrolled</span></span>|<span data-ttu-id="3e06e-116">1</span><span class="sxs-lookup"><span data-stu-id="3e06e-116">1</span></span>|<span data-ttu-id="3e06e-117">Inscrever-se o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3e06e-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="3e06e-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="3e06e-118">pendingReset</span></span>|<span data-ttu-id="3e06e-119">2</span><span class="sxs-lookup"><span data-stu-id="3e06e-119">2</span></span>|<span data-ttu-id="3e06e-120">Inscritos, mas ele está inscrito via perfil de inscrição e o perfil registrado é diferente do perfil atribuído.</span><span class="sxs-lookup"><span data-stu-id="3e06e-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="3e06e-121">Falha</span><span class="sxs-lookup"><span data-stu-id="3e06e-121">failed</span></span>|<span data-ttu-id="3e06e-122">3</span><span class="sxs-lookup"><span data-stu-id="3e06e-122">3</span></span>|<span data-ttu-id="3e06e-123">Não inscritos e não houver registro de falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="3e06e-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="3e06e-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="3e06e-124">notContacted</span></span>|<span data-ttu-id="3e06e-125">4</span><span class="sxs-lookup"><span data-stu-id="3e06e-125">4</span></span>|<span data-ttu-id="3e06e-126">Dispositivo é importado, mas não inscritos.</span><span class="sxs-lookup"><span data-stu-id="3e06e-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="3e06e-127">bloqueado</span><span class="sxs-lookup"><span data-stu-id="3e06e-127">blocked</span></span>|<span data-ttu-id="3e06e-128">5</span><span class="sxs-lookup"><span data-stu-id="3e06e-128">5</span></span>|<span data-ttu-id="3e06e-129">Dispositivo está inscrito como userless, mas seja bloqueado para mover para a inscrição do usuário porque o aplicativo falha na instalação.</span><span class="sxs-lookup"><span data-stu-id="3e06e-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





